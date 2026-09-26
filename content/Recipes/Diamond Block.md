---
tags:
  - recipes
  - recipes/blocks
  - inputs/diamond
  - inputs/diamond_ore
  - outputs/diamond_block
---

### Inputs

- 9x Diamond Ore

### Requires

- Crushing Wheel
- Automated Packing

### Outputs

- 2x Diamond Block

### Workflow Diagram

```mermaid
flowchart TD
    DiamondOre[Diamond Ore]
    Diamond[Diamond]
    DiamondBlock[Diamond Block]
    Crush(Crushing Wheels)
    Pack(Mechanical Press)
    Storage[Long Term Storage]
    CobbledDeepslate[Cobbled Deepslate]
    XPNugget[Nugget Of Experience]
    DiamondOre -->|9x| Crush
    Crush -->|18x| Diamond
    Crush -->|25% Chance +1x per ore| Diamond
    Crush -->|12% Chance +1x per ore| CobbledDeepslate
    Crush -->|75% Chance +1x per ore| XPNugget
    XPNugget --> Storage
    CobbledDeepslate --> Storage
    Diamond -->|18x| Pack
    Pack -->|2x| DiamondBlock
```