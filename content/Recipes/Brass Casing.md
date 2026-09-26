---
tags:
  - recipes
  - recipes/casings
  - inputs/logs
  - inputs/brass_ingot
  - outputs/brass_casing
---

### Inputs
- 1x Log
- 1x [[Brass Ingot]]

### Requires
- Deployer
- Mechanical Saw


### Outputs
- 1x Brass Casing


```mermaid
flowchart TD
	Log[Log]
	StrippedLog[Stripped Log]
	Casing[Brass Casing]
	Saw(Mechanical Saw)
	Deployer(Deployer: Brass Ingot)
	
	Log --> | 1x | Saw
	Saw --> | 1x | StrippedLog
	StrippedLog --> | 1x | Deployer
	Deployer --> | 1x | Casing
```
