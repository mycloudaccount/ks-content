# MagicaVoxel Character Workflow

## 🚀 Summary Workflow

1. Model the character (focus on shape)
2. Choose a limited palette
3. Apply Minecraft-style texture variation
4. Save `.vox`
5. Export `.obj` if needed
6. Commit to Git

---

## Overview

This repo contains voxel characters created in **MagicaVoxel** and stored in **Git** for version control.

The goal of this README is to provide **practical guidance** for:

* creating voxel characters
* achieving a **Minecraft-style texture look**
* exporting models for use in other tools
* keeping everything organized in source control

---

## Folder Structure

```text
/assets
  /magicavoxel
    knight.vox
    mage.vox

  /exports
    /obj
      /knight
        knight.obj
        knight.mtl
        knight.png
      /mage
        mage.obj
        mage.mtl
        mage.png
```

---

## 1. Create Models in MagicaVoxel

Start with simple, readable shapes.

### Approach

* Block out the character using basic forms (head, torso, limbs)
* Focus on **silhouette first**, not details
* Keep proportions slightly exaggerated for readability
* Zoom out often to make sure the character still “reads”

### Tips

* Think in **chunks**, not tiny voxels
* Avoid early detail — refine shape first
* Use symmetry tools initially, then break symmetry for realism

---

## 2. Use a Limited Palette

A strong voxel style depends heavily on color discipline.

### Why It Matters

* Keeps the model visually cohesive
* Makes texturing easier
* Maintains consistency across characters

### How to Do It

For each material:

* 1 base color
* 1 darker shade
* 1 lighter shade
* (optional) 1 accent

### Tips

* Reuse colors across the character
* Avoid introducing unnecessary colors
* Keep saturation controlled

---

## 3. Apply Minecraft-Style Texturing

This is where the model comes to life.

### Core Concept

Surfaces should not be perfectly flat.
Use **controlled randomness** with nearby palette colors.

---

### Step-by-Step Method

1. Paint the surface with a base color
2. Add darker and lighter variations
3. Keep most of the surface the base color
4. Use small clusters instead of full noise

---

### Target Balance

* 70–80% base color
* 10–15% darker
* 10–15% lighter

---

### Best Practices

* Break up large flat areas
* Avoid visible patterns
* Keep faces and key details clean
* Think “slightly worn,” not “random noise”

---

### Common Mistakes

* Too much variation → messy
* Too little variation → flat and lifeless
* Too many colors → inconsistent style

---

### Rule of Thumb

> Mostly flat, slightly broken up

---

## 4. Save `.vox` Source Files

The `.vox` file is your **source of truth**.

### Why It Matters

* Fully editable voxel data
* Required for future changes
* Preserves original work

### Best Practices

* Save frequently
* Use clean names:

  * `knight.vox`
  * `mage.vox`
* Never rely on exported files as your source

---

## 5. Export to `.obj` When Needed

Use OBJ exports when bringing models into other tools or engines.

---

### Expected Export Directory Structure

```text
/assets
  /magicavoxel
    knight.vox

  /exports
    /obj
      /knight
        knight.obj
        knight.mtl
        knight.png
```

---

### Structure Rules

* One folder per character
* Keep `.obj`, `.mtl`, `.png` together
* Match filenames exactly

---

### How to Export

1. Open `.vox` in MagicaVoxel
2. Export as **OBJ**

---

### Output Files

* `.obj` → geometry
* `.mtl` → materials
* `.png` → texture/palette

---

### Tips

* Export only when needed
* Re-export after changes
* Do not manually edit export files
* Treat exports as generated artifacts

---

## 6. Commit Everything to Git

Version control keeps your work safe and organized.

### What to Commit

* Always:

  * `.vox` files
* Usually:

  * `.obj`, `.mtl`, `.png`

---

### Suggested Workflow

```bash
git add assets/magicavoxel/knight.vox
git commit -m "Add knight base model"

git add assets/magicavoxel/knight.vox
git commit -m "Improve knight textures"

git add assets/exports/obj/knight/*
git commit -m "Export knight to obj"
```

---

### Why It Helps

* Track progress
* Revert mistakes
* Maintain consistency across assets

---

## Final Thoughts

The Minecraft-style look comes from:

* limited palette
* subtle randomness
* avoiding perfection

If everything is flat → it looks dead
If everything is noisy → it looks messy

The goal is right in between.
