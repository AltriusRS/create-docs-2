---
tags:
  - recipes
  - recipes/items
  - inputs/sand
  - outputs/nether_quartz
---
### Inputs
- 1x Sand

### Requires
- Bulk Haunting: soul fire
- Bulk Washing: water

### Outputs
- 12% chance: 4x Nether Quartz 
- 2% chance: 1x Gold Nugget

### Workflow Diagram



```mermaid
flowchart TD
	Sand[Sand]
	Soul[Soul Sand]
	Quartz[Nether Quartz]
	Nugg[Gold Nugget]
	Haunt(Bulk Haunting)
	Wash(Bulk Washing)
	
	Sand --> | 1x | Haunt
	Haunt --> | 1x | Soul
	Soul --> | 1x | Wash
	Wash --> |12% chance: +4|Quartz
	Wash --> |2% chance: +1|Nugg
```

