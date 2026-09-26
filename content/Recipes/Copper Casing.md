---
tags:
  - recipes
  - recipes/casings
  - inputs/logs
  - inputs/copper_ingot
  - outputs/copper_casing
---

### Inputs
- 1x Log
- 1x Copper Ingot

### Requires
- Deployer
- Mechanical Saw


### Outputs
- 1x Copper Casing


### Workflow Diagram


```mermaid
flowchart TD
	Log[Log]
	StrippedLog[Stripped Log]
	Casing[Copper Casing]
	Saw(Mechanical Saw)
	Deployer(Deployer: Copper Ingot)
	
	Log --> | 1x | Saw
	Saw --> | 1x | StrippedLog
	StrippedLog --> | 1x | Deployer
	Deployer --> | 1x | Casing
```
