---
tags:
  - recipes
  - recipes/ingots
  - inputs/copper_ingot
  - inputs/zinc_ingot
  - outputs/brass_ingot
---

### Inputs

- 1x Zinc Ingot
- 3x Copper Ingot

### Requires

- Crushing Wheel
- Automated Shapeless Crafting
- Bulk Blasting: Lava

### Outputs

- 4x Brass Ingot

### Workflow Diagram

```mermaid
flowchart TD
    ZincIngot[Zinc Ingot]
    ZincDust[Zinc Dust]
    CopperIngot[Copper Ingot]
    CopperDust[Copper Dust]
    BrassIngot[Brass Ingot]
    BrassDust[Brass Dust]
    Crush(Crushing Wheels)
    Mix(Mechanical Mixer)
    Blast(BulkBlasting)
    ZincIngot -->|x1| Crush
    CopperIngot -->|x3| Crush
    Crush -->|x1| ZincDust
    Crush -->|x3| CopperDust
    ZincDust -->|x1| Mix
    CopperDust -->|x3| Mix
    Mix -->|x4| BrassDust
    BrassDust -->|x4| Blast
    Blast -->|x4| BrassIngot
```