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
