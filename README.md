# Selections And Navigations ✅
1) Navigation:
  ``` text
  Viewport = Right Upper tab which has objects/ Modifiers on lower right
  Rotate = (MMB)
  Free move = (Shift + MMB)
  Select object then zoom on it = Numpad (.)
  ```
- FreeCam 🎥:
 ``` text
Enable Walk/Fly navig = Shift + ~
Controls = WASD, Q/E down/up, Mouse = look around, Shift = move faster
```
2) **Selection**:
- A = Select all 
- Alt + A = Deselect all  
- Shift + Click = Multi-select 
- Ctrl + I = Invert selection

3) **Mistakes**:

| **Undo**           | **Redo** | 
|------------------|-------------------------|
|  Ctrl + Z | Ctrl + Shift + Z  |
|   Edit --> UndoHistory        |  |

- **Basics**:

- Object Mode basics: Move object = ``G``, Rotate object = ``R``, Scale = ``S``
- Edit mode: Extrude = ``E``, loop cut = ``Ctrl + R``, Bevel = ``Ctrl + B``
- ViewPort: 


# Modes 🔀
| **Object Mode**                          | **Edit Mode**                               |
|------------------------------------------|---------------------------------------------|
| G = Move object                          | G = Move/slide vertices/edges/faces         |
| R = Rotate object                        | E = Extrude                                 |
| S = Scale object                         | Ctrl + R = Loop cut                         |
| Shift + A = Add new object               | Ctrl + B = Bevel                            |
| Shift + D = Duplicate object             | K = Knife tool                              |
| Tab = Switch to Edit mode                | Alt + M = Merge vertices                    |
|                                          | Alt + S = Shrink/Fatten                     |
|                                          | Tab = Switch back to Object mode            |

**Viewport**

**Viewport Modes**
- WireFrame: Display only edges of geometry without surface.
- Toggle X-ray: Transparent scene display, allow selecting through items.
- Material Preview: View material/ color of objects

## Shortcuts 🔎
# 1) ViewPort
- Numpad 1 = Front view
- Numpad 3 = Side view  
- Numpad 7 = Top view
- Numpad 5 = Toggle perspective/ortho
- Numpad (.) = Select object zoom on it


# 2) Object mode ✨
``` text
G = Grab/Move → G + X/Y/Z (axis lock) 
R = Rotate → R → 90 (90° snaps) 
S = Scale → S → 0.5 (half size) → X/Y/Z (axis) 
Shift + A = Insert parts 
Shift + D = Duplicate + move 
Tab = Edit/Object mode toggle
```

# 3) Editor Mode ⚒️
``` text
E = Extrude faces/edges/verts
Ctrl + R = Loop cut (scroll for multiples)
Ctrl + B = Bevel (scroll for segments)
G = Slide vertices (your head sculpting)
K = Knife tool (custom cuts)
Alt + M = Merge verts
Alt + S = Shrink/Fatten objects
```

# Built Tips 🧠
**Day 1**
- Made a head model using Extrude ``E in edit mode (tab)`` , scaling ``(S)``, moving vertices ``(G) in edit mode``. 
- Made body using: Bevel, scale, Duplicate, move in coordinates, 

**Day 2**
- Mirror modifier: Select a side, set cursor to midpoint, set origin to 3d cursor.
- go to modifier tab, apply mirror modifier.
- By setting object origin to midpoint/3d cursor, will mirror on other side from same distance

Analogy Mirroring modifier: ``axis -x ----0---- x`` WHERE 0 = 3d cursor.

``Made a Robot.blend, Default rig.blend, Restored Arena 4 temple like structure. Arena.blend``


**Day 3**
Learning to color a 3d model.

1) Creating a material
   - Select the object in outliner, then give it a material from material tab.
   - Rename Material to describe the object like: ``character.base.skin``
   - Shader editor enables complex material handling. material tab on right bottom is fine for simple color objects for games

# Set a particular region to x color

***

## Step 1: Make sure you’re in Edit Mode

1. Select your mesh (the whole head/body/whatever).  
2. Press `Tab` → choose **Edit Mode**.  
3. Switch to **Face Select** (the little square icon, or press `3` on the top row, not numpad). 
***

## Step 2: Create a second material

1. On the right, go to **Material Properties** (red sphere icon).  
2. You’ll see your metal material already there in the list.  
3. Click the **+** button above the material list to add a **new material slot**. 
4. With that new slot selected, click **New** to create a second material (call it “EyesRed” or whatever).  
5. Change the **Base Color** of this new material (e.g., bright red).  

At this point you have **two materials on the object**, but only the first is actually assigned to faces.
***

## Step 3: Assign that new material ONLY to selected faces

1. Still in **Edit Mode**, **Face Select**.  
2. Select only the faces you want (e.g., the eyes):  
   - Click faces one by one, or  
   - `L` over a disconnected island, or  
   - Box select with `B`.
3. In the Material list, click your **EyesRed** material so it’s highlighted.  
4. Click the **Assign** button under the material list.

Now only those selected faces use EyesRed; the rest still use the metal material.

If you **skip the “+ slot + Assign” part** and only change Base Color on the existing material, Blender updates the **same material** → whole mesh changes, exactly what you’re seeing.

# Export/Import
**Export** as obj from blender.

**Import** In rblx. It will be a mesh.

1. Select imported MeshPart in Explorer  
2. Properties panel → **CollisionFidelity** = "PreciseConvexDecomposition"  
   (Default "Box" = bad collisions → players clip through)  
3. **CanCollide** = true (unless decorative)  
4. **CanTouch** = true (for triggers/scripts)  
5. **Material** = Plastic/Neon (match Blender look)  
6. Scale/Position after import (G/R/S shortcuts work here too)
