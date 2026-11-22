# Cumulative Novice Skill List (SolidCraft CAD Study)

Running ledger of CAD skills, UI locations, and software translations a beginner has legitimately learned by working sequentially through *Mastering Autodesk Fusion (Edt. 3)* inside **SolidCraft** (`https://app.solidcraft.io/`, `v0.45.0`).

---

## Experimental Rules (Strict Novice / No-RED-Workaround Protocol)

1. **Allowed Knowledge Only:** When executing any section, the agent may rely ONLY on:
   - Natural-language comprehension of the current chapter/section instructions in the book, **plus**
   - Skills and SolidCraft UI translations already unlocked in **earlier** completed sections below.
2. **Do NOT "Fix" `RED` Gaps:** Never apply expert CAD knowledge or clever multi-step workarounds to bypass a missing, broken, or unusable feature. If a novice reading the book cannot complete a step cleanly without inventing an unmentioned workaround, **stop**, log it honestly as **`RED`**, note whether it is a textbook/ecosystem artifact or a genuine modeling blocker, and ask the tester how to proceed.
3. **Incremental Updates:** At the end of each completed section (`1.0` → `1.1` → `1.2` → Ch. 2 → …), append only the newly discovered tools and SolidCraft translations unlocked during that section.

---

## Unlocked After Ch. 1 — `1.0 The Basics` (Phase A)

- **Starting a Millimeter Design:** On the **Start** screen, click **`New design`** (`Millimeters · opens in Design`) — or `File > New Design` (`Ctrl+N`) — without needing a Part/Assembly/Hybrid selector.
- **File & Home Navigation:**
  - Top-left **Home (House) icon** opens the Start screen (`Start`, `New`, `Open...`, `Import...`, `Recover`, `Recent`, `Samples`).
  - Top-left **`File`** dropdown provides `Save` (`Ctrl+S`), `Save As...`, `Download design`, `Files in this browser...`, `Insert STEP/Mesh/Point Cloud/Design...`, `Export ...`, and `Design Properties...`.
- **Workspaces & Ribbon Layout:**
  - Top-left **`Design / Workspace ⌄`** switcher holds **`Design`**, **`Drawing`**, and **`Render`**.
  - Inside **`Design > Model`**, tool groups include `Sketch ⌄`, `Create ⌄` (e.g., `Extrude`), `Modify ⌄` (e.g., `Fillet`), `Arrange ⌄`, `Configure ⌄`, and `Construct ⌄`.
  - `Assemble`, `Insert`, `Inspect`, `Manage`, `View`, `Sheet Metal`, and `Weldments` are top-level ribbon tabs; **`Select ⌄`** (selection filters) lives inside **`View`**.
- **Browser (Model Tree), Units & Origin Planes:**
  - Left **`Browser`** panel displays the root component, **`Document Settings`** (single-click **`Units: mm`** directly to verify/change units), and **`Origin`**.
  - Default Origin planes are labeled **`XY`** (Top), **`XZ`** (Front), and **`YZ`** (Right) *(or switchable to `Top · Front · Right` in `Preferences > WORK > Design > ORIGIN`)*.
  - **Eye icons** next to `Origin` or individual axes/planes toggle visibility in the 3D viewport.
- **Timeline (`History`):** Bottom **`History`** bar holds transport controls (`Go to beginning`, `Go back one step`, `Play History`, `Go forward one step`, `Go to end`) and the blue vertical **History marker** rollback line.
- **Viewport Display & Camera Controls:**
  - Bottom floating Navigation Bar provides `Orbit`, `Pan`, `Zoom`, `Fit` (`F6`), `Look at`, `Home`, **`Visual style`** (Cube icon → **`Shaded with edges`** default), and **`Display`** (Sliders icon → **`GRAPHICS > Preset: Performance`**, **`SHOW > Grid`**, **`PROJECTION > Orthographic`**).
  - Top-right **XYZ Axis Gizmo** replaces the Fusion ViewCube: click `X`/`Y`/`Z` spheres (or opposite rings) for orthographic axis views and the small **`Home view`** house icon for Isometric view.
  - **`Mouse mapping: Fusion`** is active by default (`Wheel` = Zoom, `Middle drag` = Pan, `Shift + Middle drag` / `Right drag` = Orbit).
- **Verified Default Preferences (`Settings` Gear):**
  - `WORK > Design > ORIENTATION`: **`Z up`** (default)
  - `WORK > Sketch > DRAWING`: **`Project face edges into new sketches`** (checked) and **`The first dimension scales the drawing`** (checked)

### Known `RED` Gaps Logged in `1.0 The Basics` (Do Not Silently Work Around)
- Cloud **Hub**, **Data Panel (3x3 Waffle)**, and **Version History (`V#`)** do not exist (local/browser-storage file model only).
- **Fixed Grid & Snaps** (`50 mm` Major Spacing, `5` Minor Subdivisions, Reference Numbers) does not exist (only `Grid` On/Off and `Snap to the grid's visible crossings`).
- **`Environment: Photobooth`** and **`Exposure (0)`** do not exist in the Design Navigation Bar or Preferences.
- **Autodesk Assistant** in-app AI chat is unavailable in the web app (*"The agent chat needs the desktop app."*).

---

## Unlocked After Ch. 1 — `1.1 Classic Donut` (Phase B)

- **Creating & Editing Sketches:**
  - Click **`Design > Model > Sketch > New Sketch`**, then select an Origin plane directly under **`Browser > Origin`** (`XZ` Front, `XY` Top, `YZ` Right) — no extra `OK` click needed.
  - The right-side floating panel is named after the active sketch (e.g., `Sketch1`); **`3D Sketch`** sits inside its collapsed **`> MORE`** drawer (unchecked by default), and **`^`** minimizes the panel.
  - To **re-open an existing sketch for editing**, **double-click it under `Browser > Sketches`** (double-clicking the `History` timeline icon did not open sketch edit mode).
  - Pressing **`[Esc]`** exits only the active sketch tool; click the green **`Finish Sketch`** button (`Sketch > Exit`) to exit sketch mode.
- **Sketch Tools, Constraints & Dimensions:**
  - **`[C]`** activates **`Sketch > Create > Circle`** (stays armed across multiple circles until `[Esc]`).
  - **`Sketch > Constrain > Horizontal/Vertical`** aligns two points (e.g., Origin and circle center) automatically by proximity.
  - **`[D]`** activates **`Sketch > Constrain > Dimension`**: clicking two points sets linear distance (first dimension scales the unconstrained sketch proportionally); clicking a circle circumference creates a Diameter (`Ø`) dimension; fully constrained geometry turns **white** (`blue` = underconstrained). Double-click an existing dimension label to edit it.
  - **`Sketch > Create ⌄ > Spline > Fit Point Spline`** places smooth fit points — **right-click** (not `Enter`) to finish the spline.
- **3D Features (`Model` & `Surface`):**
  - **`Model > Create > Revolve`** auto-selects a single closed sketch profile; click **`Axis`** then **`Browser > Origin > Z`** for a 360° Z-axis revolve (`Operation: New Body`).
  - **`[E]`** opens **`Model > Create > Extrude`** (`Direction: Symmetric`, `Extent Type: All` or `Distance`, `Operation: Cut` to subtract across selected closed regions).
  - **`[F]`** opens **`Model > Modify > Fillet`** (`"click edges or faces"`, `Tangent Chain` checked by default; sharp edge loops fillet cleanly even when smooth-face selection fails).
  - **`Model > Modify ⌄ > Faces > Split Face`** splits faces **only with a plane or planar face** (e.g., `Browser > Origin > XY`); **`Surface > Create > Extrude`** can extrude an open 2D spline symmetrically into a surface body, though `Split Face` still requires a planar tool.
- **Materials & Custom Appearances (`[A]`):**
  - **`[A]`** opens **`Manage > Materials > Appearance`** (leaves ribbon on `Manage`, so switch back to **`Model`** before clicking `New Sketch`).
  - **`Apply To`** supports **`Bodies`** and **`Faces`** (per-face overrides preserve separate body appearances like `Wood - Oak` on bite cut walls).
  - Customizing a `LOCAL LIBRARY` swatch (e.g., `Steel - Satin`) via the **`Color`** box → **`Hex`** tab (e.g., `#f00af0` for `RGB 240, 10, 240`) works reliably (`U8` numeric `R` text box ignored direct typing).
- **Parametric Rebuild:** Editing an early sketch dimension (`Browser > Sketches > Sketch1`) triggers downstream timeline recompute (`History` / `Browser > Features` shows yellow `!` fallback warnings if topological edge matching falls back to geometry).

### Known `RED` Gaps Logged in `1.1 Classic Donut` (Do Not Silently Work Around)
- **Procedural Wood-Grain Texture & `Scale` (`44%`):** `Wood - Oak` in `Appearance` (`LOCAL LIBRARY`) renders as a uniform PBR color swatch with no texture pattern or UV `Scale` control (**cross-software textbook / material-library artifact**).
- **`Split Face` with Open 2D Sketch Spline:** `Model > Modify ⌄ > Faces > Split Face` restricts `Splitting tool` to `"a plane or planar face"` and rejects both 2D sketch splines (`Sketch2`) and curved surface extrudes (`Body2`) (**true CAD modeling blocker**).
- **`Press Pull [Q]` / `Offset Face` on Curved/Split Torus Face:** `Press Pull [Q]` delegates to `Offset Face` rather than Fusion's `New Offset` stepped-wall offset, triggering an SMLib `"how far its neighbours extend to meet it has no certified bound"` kernel failure on the torus (**true CAD modeling blocker**).
