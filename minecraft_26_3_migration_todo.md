# The Vervada (Main Pack) - 26.3 Migration & Missing Features To-Do

Based on the analysis of the *main* Vervada resource pack, below is a comprehensive list of tasks required to fully support modern Minecraft up to the 26.3 release. This covers not just plants, but also building blocks, custom models, and CTM overlays.

## Upcoming 26.3 Release (Dappled Forest)
- [ ] **Flora & Plants**:
  - [ ] Poplar Sapling & Potted Poplar Sapling
  - [ ] Poplar Leaves
  - [ ] Shelf Mushroom
  - [ ] Red Shrub & Potted Red Shrub
- [ ] **Wood Building Blocks** (Models need to match the custom style of existing wood types):
  - [ ] Poplar Door (Top/Bottom, Left/Right, Open/Closed)
  - [ ] Poplar Trapdoor (Top/Bottom, Open/Closed)
  - [ ] Poplar Fence (Inventory, Post, Side)
  - [ ] Poplar Fence Gate (Open/Closed, Wall variations)
  - [ ] Poplar Sign

## 1.21 / 1.20 Catch-up & Missing Custom Models
The pack does a fantastic job with 1.21 features (like Copper models and the Crafter), but some items from recent updates were missed in the main pack:

- [ ] **Pale Oak (Winter Drop)**: 
  - [ ] Pale Oak Leaves
  - [ ] Pale Hanging Moss *(Note: This exists in the 3D-plants add-on, but is missing in the main pack)*
  - [ ] Pale Oak Door & Trapdoor models
  - [ ] Pale Oak Fence & Fence Gate models
  - [ ] Pale Oak Sign
- [ ] **Missing Signs**: While oak, birch, etc., have custom `.json` models, the newer wood types are missing them:
  - [ ] Bamboo Sign
  - [ ] Cherry Sign
  - [ ] Mangrove Sign
- [ ] **Missing Bamboo Fences**: 
  - [ ] Bamboo Fence & Fence Gate models *(Doors and Trapdoors are present!)*
- [ ] **Hanging Signs**: 
  - [ ] Custom models for Hanging Signs for *all* wood types are currently absent. 
- [ ] **Tricky Trials (Optional)**:
  - [ ] Vault / Ominous Vault model *(A `template_vault.json` exists, but no specific block models for it)*
  - [ ] Heavy Core model

## Missing Vanilla Flora & Crops
Since the main pack includes the 3D crops and flowers feature, the following plants still lack custom 3D models. *(Note: Kelp, Wheat, and Twisting Vines were intentionally excluded per the README)*:
- [ ] Seagrass & Tall Seagrass
- [ ] Sea Pickle
- [ ] Glow Lichen
- [ ] Chorus Plant & Flower
- [ ] Spore Blossom
- [ ] Moss Carpet
- [ ] Bamboo Stalk / Leaves *(Only the `bamboo_sapling` is currently modelled)*

## CTM Overlay Updates Needed
The main pack features extensive Optifine/Continuity Connected Textures (CTM) overlays across 11 different blocks (bricks, coarse_dirt, concrete, dirt, grass_block, gravel, red_sand, red_sandstone, sand, sandstone, terracotta). 
- [ ] **Update `matchBlocks`**: Ensure that all new solid blocks from 1.21 (like `resin_block`, `pale_oak_wood`) and 26.3 (`poplar_wood`, stripped variants) are added to the `matchBlocks` property in all 11 of these overlay directories so textures blend smoothly against them.
- [ ] **New Soils**: Ensure any newly added Dappled Forest soil blocks are added to the base overlay lists (e.g., `connectBlocks` or base overlay target lists) if they require the same CTM smoothing as standard grass/dirt.
