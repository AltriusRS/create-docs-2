---
tags:
  - recipes
  - inputs/crimsite
  - outputs/redstone_dust
  - outputs/iron_nuggets
---
### Inputs
- 64x Crimsite

### Requires
- Crushing Wheels
- Bulk Washing: Water


### Outputs

> [!info]  
> These outputs are based on random chance. These numbers are based on expected values derived from long-term averages.

- 256x Iron Nugget
- 19x Redstone Dust

```mermaid
flowchart TD
	CR[Crimsite]
	IC[Iron Clump]
	IN[Iron Nugget]
	RD[Redstone Dust]
	CW(Crushing Wheels)
	BW(Bulk Washing: Water)
	
	CR --> | 1x | CW
	CW --> | 40% chance: 1x | IC
	CW --> | 40% chance: 1x | IN
	IC --> | 1x | BW
	BW --> | 9x | IN
	BW --> | 75% chance: 1x | RD
```
