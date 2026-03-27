## 1. Create Models in MagicaVoxel

Start with simple, readable shapes.

### Approach

- Block out the character using basic forms (head, torso, limbs)
- Focus on **silhouette first**, not details
- Keep proportions slightly exaggerated for readability
- Zoom out often to make sure the character still “reads”

### Tips

- Think in **chunks**, not tiny voxels
- Avoid early detail — refine shape first
- Use symmetry tools where helpful, then break symmetry later for realism

---

## 2. Use a Limited Palette

A strong voxel style depends heavily on color discipline.

### Why It Matters

- Keeps the model visually cohesive
- Makes texturing easier
- Helps maintain a consistent art style across characters

### How to Do It

For each material (skin, cloth, metal, etc.):

- Choose:
  - 1 base color
  - 1 darker shade
  - 1 lighter shade
  - (optional) 1 accent

### Tips

- Reuse colors across different parts of the character
- Avoid introducing new colors unless necessary
- Keep saturation and brightness controlled

---

## 3. Apply Minecraft-Style Texturing

This is where the model comes to life.

### Core Concept

Surfaces should not be perfectly flat.  
Instead, use **controlled randomness** with nearby palette colors.

### Process

1. Paint the entire surface with a base color  
2. Add darker and lighter pixels sparingly  
3. Keep most of the surface the base color  
4. Use small clusters instead of pure noise  

### Target Balance

- ~70–80% base color  
- ~10–15% darker  
- ~10–15% lighter  

### Tips

- Break up large flat areas
- Avoid patterns or symmetry in texture
- Keep important areas (faces, eyes) clean and simple

---

## 4. Save `.vox` Source Files

The `.vox` file is your **source of truth**.

### Why It Matters

- Contains full voxel data
- Editable at any time
- Required for future changes or improvements

### Best Practices

- Save frequently while working
- Keep clean filenames:
  - `knight.vox`
  - `mage.vox`
- Do not rely on exported files as your source

---

## 5. Export to `.obj` When Needed

Use OBJ exports when bringing models into other tools or engines.

### How to Export

1. Open your `.vox` file
2. Use MagicaVoxel export
3. Choose **OBJ format**

### Output Files

- `.obj` → geometry
- `.mtl` → materials
- `.png` → texture/palette

### Tips

- Export only when needed (don’t spam exports)
- Keep exports organized in a separate folder
- Re-export after making changes to the `.vox` file

---

## 6. Commit Everything to Git

Version control keeps your work safe and organized.

### What to Commit

- Always:
  - `.vox` source files
- Usually:
  - exported `.obj`, `.mtl`, `.png`

### Suggested Workflow

- Commit after meaningful changes
- Use clear commit messages:
  - `add base character model`
  - `improve palette and textures`
  - `export character to obj`

### Why It Helps

- Track progress over time
- Revert mistakes easily
- Maintain consistency across multiple characters

---

## Summary Workflow

1. Model the character (focus on shape)
2. Choose a limited palette
3. Apply Minecraft-style texture variation
4. Save `.vox`
5. Export `.obj` if needed
6. Commit to Git
