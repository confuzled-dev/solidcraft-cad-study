# Session 3 Setup & Viewport Notes (Phase B: `1.1 Classic Donut`)

Prepared from Phase A (`1.0 The Basics`) observations on **SolidCraft `v0.45.0`** (`https://app.solidcraft.io/`) and the live Antigravity split-screen layout on a large high-DPI display.

---

## 1. Browser & Recording Setup (Replacing `1280x720`)

- **Do NOT resize or emulate `1280x720` via `setViewportSize`.** Forcing `1280x720` triggered the `"Ensure 1280x720 viewport..."` banner in the split-screen pane and cramped toolbars/popovers. Use the **live browser pane dimensions as-is** so the browser subagent and OBS recording match 1:1.
- **Verified High-DPI Split-Pane Layout:**
  - Maximize Antigravity and keep the divider around **25–30% Chat** / **70–75% SolidCraft browser pane** (optionally `Ctrl + -` once or twice if extra room is desired).
  - Before hitting Record, verify `Weldments` and `Press Pull` fit on the `Design → Model` ribbon without truncation.
- **Desktop Multitasking While Recording (OBS):**
  - Configure OBS with **Window Capture** targeting Antigravity (not full Display Capture) so other windows never enter the recording.
  - Keep Antigravity **unminimized on the same workspace** while working elsewhere on your screen so OBS frames and SolidCraft's WebGL canvas are not throttled.
  - The browser subagent operates directly inside the webview and does not steal your physical cursor or keyboard (just avoid clicking inside the SolidCraft pane mid-step).
- **Optional In-App Space Savers (if needed):**
  - UI scale fallback: `Settings (Gear) → LOOK → Appearance → SCALE AND TEXT → 75%` (default is `100%`).
  - Temporarily collapse the left `Browser` panel using its `^` chevron if feature dialogs cover the viewport, then re-expand when selecting items in the tree.

---

## 2. Clean Start Checklist

1. Open `https://app.solidcraft.io/`.
2. If the **`Recover unsaved work?`** modal appears (`"Untitled" had unsaved changes when this page last closed.`), click **`Discard`** to start fresh.
3. Click **`New design`** (`Millimeters · opens in Design`).
4. **Verified `1.0` defaults already active out of the box (no setup clicks needed):**
   - `Preferences → INPUT → Navigation → Mouse mapping: Fusion`
   - `Browser → Document Settings → Units: mm`
   - `Preferences → WORK → Design → ORIENTATION: Z up`
   - `Display → PROJECTION: Orthographic`
   - `Visual style: Shaded with edges`
   - `Display → GRAPHICS → Preset: Performance`
   - `Preferences → WORK → Sketch → DRAWING`: `Project face edges into new sketches` (**checked**) and `The first dimension scales the drawing` (**checked**)

---

## 3. Strict Novice & No-RED-Workaround Rules (+ Harness Notes)

- **Allowed Prior Knowledge:** Use **only** natural-language understanding of Chapter `1.1 Classic Donut` plus the skills explicitly unlocked after `1.0 The Basics` in [novice_skill_list.md](../novice_skill_list.md). Do **not** pre-feed Phase B tool paths (`Revolve`, `Spline`, `Split Face`, `Press Pull`, Appearance locations, etc.)—let Session 3 discover them organically from the book's instructions.
- **Zero Workarounds for `RED` Blockers:** Do **not** "fix" or quietly route around any missing/broken feature using outside CAD expertise. If a novice following the book hits a `RED` failure, document it immediately, log it as `RED`, and ask the tester how to proceed.
- **Automation Harness Notes (Non-CAD):**
  - During Phase A, synthetic `mouse.wheel` events in Playwright did not zoom the WASM canvas; use the bottom Navigation Bar **`Zoom`** tool or **`Fit` (`F6`)** if automated zooming is needed.
  - Close the `app.solidcraft.io` tab when Phase B finishes to unload WebGL/WASM and free GPU resources.

---

## 4. Ready-to-Paste Session 3 Prompt Snippets

```markdown
# BROWSER SETUP (LIVE PANE — DO NOT RESIZE)
1. Open `https://app.solidcraft.io` in the browser (or reuse the open Start tab).
2. **Do NOT resize the browser viewport** (`setViewportSize` / `1280x720` disabled) — use the live Antigravity split-screen browser pane dimensions as-is so the subagent and OBS recording match 1:1.
3. If `Recover unsaved work?` appears, click `Discard`, then pause and ask me **"Ready to record?"** on the clean Start screen before clicking `New design` (`Millimeters · opens in Design`).

# STRICT NOVICE & NO-RED-WORKAROUND RULES
- Act strictly as a CAD novice with **zero outside CAD expertise**, using only natural-language comprehension of `1.1 Classic Donut` and the prior skills listed in `./demo_runs/novice_skill_list.md`.
- **Never "fix" or invent workarounds for `RED` blockers.** If any instruction cannot be completed naturally through SolidCraft's UI using book concepts + `novice_skill_list.md`, STOP that step, log it as `RED`, and ask me how to proceed.
- Update `./demo_runs/novice_skill_list.md` at the end of Phase B with only the SolidCraft skills successfully learned in `1.1 Classic Donut`.
```
