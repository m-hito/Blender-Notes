# Selections And Navigations ✅
- Navigation:
  ``` text
  Rotate = (MMB)
  Free move = (Shift + MMB)
  Select object then zoom on it = Numpad (.)
  ```
- FreeCam 🎥:
 ``` text
Enable Walk/Fly navig = Shift + ~
Controls = WASD, Q/E down/up, Mouse = look around, Shift = move faster
```
- Object Mode basics: Move object = ``G``, Rotate object = ``R``, Scale = ``S``
- Edit mode: Extrude = ``E``, loop cut = ``Ctrl + R``, Bevel = ``Ctrl + B``

# Modes 🔀
**Object mode** 

**Editor mode** 

**Viewport Shading**
- WireFrame: Display only edges of geometry without surface.
- Toggle X-ray: Transparent scene display, allow selecting through items.


# Object mode ✨
``` text
G = Grab/Move → G + X/Y/Z (axis lock) 
R = Rotate → R → 90 (90° snaps) 
S = Scale → S → 0.5 (half size) → X/Y/Z (axis) 
Shift + A = Insert parts 
Shift + D = Duplicate + move 
Tab = Edit/Object mode toggle
```

# Editor Mode ⚒️
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
 Made a head model using Extrude ``E in edit mode (tab)`` , scaling ``(S)``, moving vertices ``(G) in edit mode``. 

Made body using: Bevel, scale, Duplicate, move in coordinates, 


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
