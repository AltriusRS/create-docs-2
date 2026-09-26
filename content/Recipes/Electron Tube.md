---
tags:
  - recipes
  - recipes/items
  - inputs/nether_quartz
  - inputs/redstone
  - inputs/iron_ingot
  - outputs/electron_tube
---
### Inputs
- 8x Redstone Dust
- 1x [[Nether Quartz]]
- 1x Iron Ingot

### Requires
- Mechanical Press
- Mechnical Grindstone
- Mechanical Crafter

### Outputs
- 1x Electron Tube



### Workflow Diagram

```mermaid
flowchart TD
	RD[Redstone Dust]
	NQ[Nether Quartz]
	II[Iron Ingot]
	IP[Iron Plate]
	RQ[Rose Quartz]
	PRQ[Polished Rose Quartz]
	ET[Electron Tube]
	
	MP(Mechanical Press)
	MG(Mechanical Grindstone)
	MC-RQ(Mechanical Crafter: Rose Quartz)
	MC-ET(Mechanical Crafter: Electron Tube)
	
	RD --> | 8x | MC-RQ
	NQ --> | 1x | MC-RQ
	MC-RQ --> | 1x | RQ
	RQ --> | 1x | MG
	MG --> | 1x | PRQ
	PRQ --> | 1x | MC-ET
	
	II --> | 1x | MP
	MP --> | 1x | IP
	IP --> | 1x | MC-ET
	
	MC-ET --> | 1x | ET
```