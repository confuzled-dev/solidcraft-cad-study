Thinking...
Convert raw text from two Autodesk Fusion course chapters into a clean Markdown checklist.
`step_plan.md`.

        *   *Phase A (1.0 The Basics):* UI elements, panels, menus, workspace concepts, preferences (Hub, Project, Part, Menus, Data Panel, Browser, Timeline, Navigation Bar, Origin/Grid, Preferences/Units).
        *   *Phase B (1.1 Classic Donut):* Sequential modeling steps (mm, exact tools/shortcuts, dimensions).
        *   *Critical Rule:* If a dimension/diagram is mentioned but not numerically specified in the text, use `[CHECK FIGURE - PAGE X]`.
        *   *Ending:* Propose 1 specific early sketch dimension to change for a Parametric Rebuild Test.
Only clean Markdown.

    *   *Context:* Intro to Fusion, Hubs, Projects, Designs.
    *   *Key Elements:*
        *   Hub (Organization of projects/data).
        *   Projects: Part Design (single object), Assembly Design (multiple parts in separate files), Hybrid Design (multiple parts in one file).
        *   Origin: Central point, small white dot.
        *   Data Panel (3x3 grid/Waffle): Folders, subfolders, House icon (main menu), Teams, Hub names, Version History (V#), Upload button.
        *   Workspace: Design (current), Render, Generative Design, Simulation, Manufacture.
        *   Toolbar: Create, Modify, Assemble, Configure, Construct, Inspect, Insert, Select.
        *   Create Menu: Turning 2D Sketch to 3D Body (e.g., Extrude).
        *   Modify Menu: Changing 3D Body (e.g., Fillet).
        *   Browser: Units, 3D objects, Construction Planes, 2D Sketches.
        *   Units: mm (set via Document Settings/Triangle icon).
        *   Origin Planes: Front (XZ), Right (YZ), Top (XY).
        *   Eye Icons: Visibility (Planes, Axes, Origin).
        *   Timeline: Bottom left, Features, History Marker, Play/Rewind/Fast Forward.
        *   Navigation Bar: Bottom middle, Visual Style (Shaded with Visible Edges Only), Environment (Photobooth), Graphics Preset (Performance), Camera (Orthographic), Grid (Fixed, Major Spacing: 50 mm, Minor Subdivisions: 5).
        *   Mouse Navigation: Scroll wheel (Zoom), Click & Hold (Pan), Shift + Scroll Wheel (Orbit).
        *   ViewCube: Top right, House icon (Isometric View), Faces (Top, Front, etc.).
        *   Autodesk Assistant: AI help tool.
        *   Preferences: Profile icon/Initials, General (Default Modeling Orientation: Z Up), Design (Auto project edges, Auto project geometry, Scale entire sketch at first dimension), Material (Physical Material, Appearance, Exposure: 0).

    *   *Sequence:*
        1.  Units: mm.
        2.  Create Sketch: Front Plane (XZ).
        3.  Sketch Palette: Check 3D Sketch (unchecked), Minimize.
        4.  Circle: Press [C], center near X-Axis, [Esc].
        5.  Horizontal Constraint: Navigate to Constraints >> Horizontal/Vertical, Select Origin & circle center, [Esc].
        6.  Dimension (Center): Press [D], Origin to circle center, type 40.
        7.  Dimension (Diameter): Circle circumference, type 20.
        8.  Finish Sketch: [Esc] or Finish Sketch button.
        9.  View: House icon (Isometric View).
        10. Revolve: Create >> Revolve, Circle (Profile), Z-Axis (Axis).
        11. Edit Sketch: Right-click Sketch1 >> Edit Sketch (or Double-click).
        12. Dimension Update: Circle diameter, type 40.
        13. Finish Sketch.
        14. Appearance: [A], Wood >> Oak (Download), Drag onto Donut, Scale 44%.
        15. New Sketch: Front Plane (XZ).
        16. Spline: Create >> Spline >> Fit Point, 6 times above/below X-Axis, [Enter] each.
        17. Finish Sketch.
        18. Split Face: Modify >> Split Face, Donut body, Spline Sketch.
        19. New Sketch: Top Plane (XY).
        20. Circles (Bite): Press [C], 3 circles near outer edge, [Esc] each.
        21. Finish Sketch.
        22. Extrude: Create >> Extrude (or [E]), 5 overlapping circles, Direction: Symmetric, [OK].
        23. Press Pull: Modify >> Press Pull (or [Q]), Top surface, Offset Distance 2.0 mm.
        24. Fillet: Modify >> Fillet (or [F]), Top icing surface, Radius 1.9 mm.
        25. Custom Appearance: [A], Steel, Color (RGB: 240, 10, 240), Apply to: Faces, Drag to top face and filleted edges.

    *   *Self-Correction during drafting:*
        *   Check for "Check Figure": In the "Fit Point Spline" step, it says "above and below the X-axis six times". It doesn't give specific numbers like 10mm or 20mm. It refers to the visual look. So, I'll keep the "6 times" but note the visual description.
        *   Check for "Fit Point Spline" specific dimensions: The text says "click above and below the X-axis six times". Since no specific mm value is given for each point, it relies on the visual. I should ensure the "6 times" is there.
        *   Check for Circle "Bite" dimensions: "3 circles... do not need to be any exact size". This means no specific number, just "3 circles."

    *   *Phase A Checklist Construction:*
        *   [ ] Hub
        *   [ ] Project Types: Part Design, Assembly Design, Hybrid Design
        *   [ ] Data Panel (The Waffle)
        *   [ ] House Icon (Main Menu)
        *   [ ] Teams & Shared Projects
        *   [ ] Version History (V#)
        *   [ ] Design Workspace
        *   [ ] Toolbar (Create, Modify, Assemble, Configure, Construct, Inspect, Insert, Select)
        *   [ ] Browser
        *   [ ] Document Settings (Units)
        *   [ ] Origin Planes (Front/XZ, Right/YZ, Top/XY)
        *   [ ] Eye Icons (Visibility)
        *   [ ] Timeline (History Marker, Play/Rewind/Fast Forward)
        *   [ ] Navigation Bar
        *   [ ] Visual Style (Shaded with Visible Edges Only)
        *   [ ] Environment (Photobooth)
        *   [ ] Graphics Preset (Performance)
        *   [ ] Camera (Orthographic)
        *   [ ] Grid & Snaps (Fixed, Major: 50 mm, Minor: 5, Reference Numbers: Unchecked)
        *   [ ] ViewCube (House Icon/Isometric)
        *   [ ] Autodesk Assistant
        *   [ ] Preferences (General, Design, Material, Exposure: 0)

    *   *Phase B Checklist Construction (Sequence):*
        *   [ ] Verify Units: mm
        *   [ ] Create Sketch: Front Plane (XZ)
        *   [ ] Sketch Palette: Uncheck "3D Sketch" and minimize
        *   [ ] Circle: [C], Place near X-Axis
        *   [ ] Constraint: Constraints > Horizontal/Vertical, Origin & Circle Center
        *   [ ] Dimension (Center): [D], Origin to Circle Center = 40 mm
        *   [ ] Dimension (Diameter): Circle diameter = 20 mm
        *   [ ] Finish Sketch
        *   [ ] View: Isometric (House Icon)
        *   [ ] Revolve: Create > Revolve, Circle (Profile), Z-Axis (Axis)
        *   [ ] Edit Sketch: Right-click/Double-click Sketch 1
        *   [ ] Update Dimension: Circle diameter = 40 mm
        *   [ ] Finish Sketch
        *   [ ] Appearance: [A], Wood > Oak, Drag onto Donut, Scale 44%
        *   [ ] New Sketch: Front Plane (XZ)
        *   [ ] Spline: Create > Spline > Fit Point, 6 times above and below X-Axis (6 fit points in a gentle wave starting outside one side of the donut and ending outside the other so it spans across the face; press Enter, not Esc, to finish)
        *   [ ] Finish Sketch
        *   [ ] Split Face: Modify > Split Face, Donut Body, Spline Sketch
        *   [ ] New Sketch: Top Plane (XY)
        *   [ ] Circles: [C], 3 overlapping circles near outer edge
        *   [ ] Finish Sketch
        *   [ ] Extrude: [E], Select 5 overlapping circles, Direction: Symmetric
        *   [ ] Press Pull: [Q], Top surface, Offset Distance: 2.0 mm
        *   [ ] Fillet: [F], Top icing surface, Radius: 1.9 mm
        *   [ ] Custom Appearance: [A], Steel, Color (RGB: 240, 10, 240), Apply to: Faces (Top/Filleted edges)

    *   *Parametric Rebuild Test:*
        *   Initial Change: Change the circle's original diameter from 20 mm to 30 mm. (Wait, let me check the flow).
        *   Original sequence: Start at 20mm -> Revolve -> Update to 40mm.
        *   Proposed Change: Change the *original* diameter (Step 7) from 20 mm to 30 mm.

    *   *Check:* Did I include all UI elements from Phase A? Yes.
    *   *Check:* Are all steps in Phase B sequential? Yes.
    *   *Check:* Are shortcuts/tools exact? Yes (e.g., [C], [D], Create > Revolve).
    *   *Check:* Are dimensions exact? Yes (e.g., 40, 20, 2.0, 1.9).
    *   *Check:* [CHECK FIGURE] placement?
        *   Spline: "above and below the X-axis six times" (No specific mm value provided for the vertical height of each point).
    *   *Check:* Clean Markdown? Yes.
...done thinking.

# step_plan.md

## Phase A: 1.0 The Basics (UI & Functions Checklist)
- [ ] **Hub**: Project and data organization
- [ ] **Project Types**: Part Design, Assembly Design, and Hybrid Design
- [ ] **Data Panel (The Waffle)**: 3x3 grid for folders, subfolders, and Teams
- [ ] **House Icon**: Return to main menu in Data Panel
- [ ] **Version History**: Tracking changes via V#
- [ ] **Upload Button**: Importing external files (STEP, SolidWorks, etc.)
- [ ] **Workspaces**: Design (Active), Render, Generative Design, Simulation, and Manufacture
- [ ] **Design Toolbar**: Create, Modify, Assemble, Configure, Construct, Inspect, Insert, and Select
- [ ] **Browser**: Displaying Units, 3D objects, Construction Planes, and 2D Sketches
- [ ] **Document Settings**: Accessing the Triangle icon for Units
- [ ] **Units**: Set to millimeters (mm)
- [ ] **Origin Planes**: Front (XZ), Right (YZ), and Top (XY)
- [ ] **Eye Icons**: Toggle visibility of Planes, Axes, and Origin
- [ ] **Timeline**: Features, History Marker, and Play/Rewind/Fast Forward buttons
- [ ] **Navigation Bar**: Visual Style (Shaded with Visible Edges Only), Environment (Photobooth), Graphics Preset (Performance), and Camera (Orthographic)
- [ ] **Grid & Snaps**: Fixed Grid, Major Grid Spacing (50 mm), Minor Subdivisions (5), and Reference Numbers (Unchecked)
- [ ] **Mouse Navigation**: Scroll Wheel (Zoom), Click & Hold (Pan), Shift + Scroll Wheel (Orbit)
- [ ] **ViewCube**: Clickable faces/edges and the House Icon (Isometric View)
- [ ] **Autodesk Assistant**: AI help tool
- [ ] **Preferences**: 
    - [ ] **General**: Default Modeling Orientation (Z Up)
    - [ ] **Design**: Auto project edges on reference, Auto project geometry on active sketch plane, Scale entire sketch at first dimension
    - [ ] **Material**: Physical Material, Appearance, and Exposure (0)

## Phase B: 1.1 Classic Donut (Sequential Modeling Steps)
- [ ] **Units**: Verify set to mm
- [ ] **Create Sketch**: Select Front Plane (XZ)
- [ ] **Sketch Palette**: Uncheck "3D Sketch" and minimize
- [ ] **Circle**: Press [C], Place near X-Axis
- [ ] **Constraint**: Constraints > Horizontal/Vertical, select Origin and Circle Center
- [ ] **Dimension (Center)**: Press [D], select Origin and Circle Center, set to 40 mm
- [ ] **Dimension (Diameter)**: Select Circle circumference, set to 20 mm
- [ ] **Finish Sketch**: Click button or press [Esc]
- [ ] **View**: Click House Icon (Isometric View)
- [ ] **Revolve**: Create > Revolve, Profile (Circle), Axis (Z-Axis)
- [ ] **Edit Sketch**: Right-click/Double-click Sketch 1
- [ ] **Update Diameter**: Double-click diameter dimension, set to 40 mm
- [ ] **Finish Sketch**
- [ ] **Appearance**: Press [A], select Wood > Oak, drag onto Donut, set Scale to 44%
- [ ] **New Sketch**: Select Front Plane (XZ)
- [ ] **Spline**: Create > Spline > Fit Point, click above and below X-Axis six times (6 fit points in a gentle wave starting outside one side of the donut and ending outside the other so it spans across the face; press Enter, not Esc, to finish)
- [ ] **Finish Sketch**
- [ ] **Split Face**: Modify > Split Face, select Donut body and Spline Sketch
- [ ] **New Sketch**: Select Top Plane (XY)
- [ ] **Circles (Bite)**: Press [C], draw 3 overlapping circles near outer edge
- [ ] **Finish Sketch**
- [ ] **Extrude**: Press [E], select 5 overlapping circles, set Direction to Symmetric
- [ ] **Press Pull**: Modify > Press Pull [Q], select top surface, set Offset Distance to 2.0 mm
- [ ] **Fillet**: Modify > Fillet [F], select top icing surface, set Radius to 1.9 mm
- [ ] **Custom Appearance**: Press [A], select Steel, set Color to RGB (240, 10, 240), set Apply To: Faces, drag onto top and filleted faces

**Parametric Rebuild Test:** 
Change the initial Circle Diameter (Step 7) from 20 mm to 30 mm.

