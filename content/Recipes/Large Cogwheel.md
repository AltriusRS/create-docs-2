---
tags:
  - recipes
  - recipes/blocks
  - inputs/small_cogwheel
  - inputs/wooden_planks
  - outputs/large_cogwheel
---
### Inputs
- 1x [[Small Cogwheel]]
- 1x Wooden Planks

### Requires
- Deployer

### Outputs
- 1x Large Cogwheel

```mermaid
flowchart TD
	LargeCog[Large Cogwheel]
	SmallCog[Small Cogwheel]
	Deployer(Deployer: Wooden Planks)
	
	SmallCog --> | 1x | Deployer
	Deployer --> | 1x | LargeCog

```
