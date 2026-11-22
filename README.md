# SolidCraft CAD Study

A strict-novice validation study testing how cleanly a CAD beginner can follow *Mastering Autodesk Fusion (Edt. 3)* inside **[SolidCraft](https://app.solidcraft.io/)** (`v0.45.0`) using only standard UI menus, icons, dialogs, and skills legitimately learned in earlier sections — without expert CAD workarounds.

---

## Validation Results (Chapter 1)

| Section | Focus | Items Evaluated | GREEN | YELLOW | RED | Log |
| :--- | :--- | :---: | :---: | :---: | :---: | :--- |
| **Phase A — `1.0 The Basics`** | Workspace, Navigation, Preferences, Browser, Timeline, Materials | 25 | 4 | 15 | 6 | [phase_a_log.md](demo_runs/ch1_basics_and_donut/phase_a_log.md) |
| **Phase B — `1.1 Classic Donut`** | Sequential 3D Modeling (Steps 1–25) | 25 | 17 | 5 | 3 | [phase_b_log.md](demo_runs/ch1_basics_and_donut/phase_b_log.md) |
| **Phase B — Parametric Rebuild Test** | Edit `Sketch1` Circle Diameter (`40 mm` → `30 mm`) | 1 | 0 | 1 | 0 | [phase_b_log.md](demo_runs/ch1_basics_and_donut/phase_b_log.md) |
| **Phase B Combined Total** | Modeling Steps 1–25 + Parametric Rebuild Test | **26** | **17** | **6** | **3** | [phase_b_log.md](demo_runs/ch1_basics_and_donut/phase_b_log.md) |

### Key Findings
- **Strong Fusion Muscle-Memory Compatibility:** SolidCraft defaults out of the box to `Mouse mapping: Fusion`, `Z up`, `mm` units, `Orthographic` projection, `Shaded with edges`, `Project face edges into new sketches`, and `The first dimension scales the drawing`. Core 2D sketching (`[C]`, `[D]`, `Horizontal/Vertical`), `Revolve`, symmetric `Cut` `Extrude`, `Fillet` (`[F]`), and per-face custom appearances (`[A]`, `Apply To: Faces`) transfer cleanly.
- **True CAD Modeling Blockers Observed (`v0.45.0`):**
  - **`Split Face` Planar-Only Restriction (Phase B Step 18):** `Model > Modify ⌄ > Faces > Split Face` restricts `Splitting tool` to *"a plane or planar face"*, rejecting both open 2D sketch splines (`Sketch2`) and symmetric `Surface > Extrude` wavy surfaces (`Body2`).
  - **`Press Pull [Q]` → `Offset Face` SMLib Error (Phase B Step 23):** Unlike Fusion's `New Offset` stepped-wall behavior, SolidCraft's `Press Pull [Q]` delegates to `Offset Face` and throws an SMLib `"how far its neighbours extend to meet it has no certified bound"` error on the curved/split torus.
- **Cross-Software Textbook & Ecosystem Artifacts:**
  - Cloud `Hub`, `Data Panel (3x3 Waffle)`, `Version History (V#)`, `Photobooth` / `Exposure (0)`, fixed `50 mm / 5` grid subdivisions, in-browser AI Assistant, and procedural material texture `Scale` (`44%` on `Wood - Oak`) do not exist in the web app.

---

## Project Structure

- [demo_runs/novice_skill_list.md](demo_runs/novice_skill_list.md) — Cumulative ledger of SolidCraft skills and UI translations unlocked section-by-section, plus documented `RED` gaps.
- [demo_runs/ch1_basics_and_donut/step_plan.md](demo_runs/ch1_basics_and_donut/step_plan.md) — Sequential validation plan for Phase A (`1.0 The Basics`), Phase B (`1.1 Classic Donut`), and the Parametric Rebuild Test.
- [demo_runs/ch1_basics_and_donut/phase_a_log.md](demo_runs/ch1_basics_and_donut/phase_a_log.md) — Phase A feature-by-feature comparison table and rewrite notes.
- [demo_runs/ch1_basics_and_donut/phase_b_log.md](demo_runs/ch1_basics_and_donut/phase_b_log.md) — Phase B modeling log, diagnostics, book rewrites, and Parametric Rebuild Test results.
- [demo_runs/ch1_basics_and_donut/session3_setup_notes.md](demo_runs/ch1_basics_and_donut/session3_setup_notes.md) — Live-pane viewport and OBS capture notes.
- [demo_runs/ch1_basics_and_donut/screenshots/](demo_runs/ch1_basics_and_donut/screenshots/) — Verification screenshots for Phase A (`phaseA_*.png`) and Phase B (`phaseB_*.png`).

> **Note:** Copyrighted textbook PDFs (`pdfs/`), native Fusion source files (`*.f3d`, `*.f3z`), and raw text extracts (`*_raw.txt`) are excluded from version control via `.gitignore`.
