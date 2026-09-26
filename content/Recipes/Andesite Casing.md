---
tags:
  - recipes
  - recipes/casings
  - inputs/logs
  - inputs/andesite_alloy
  - outputs/andesite_casing
---

### Inputs
- 1x Log
- 1x Andesite Alloy

### Requires
- Deployer
- Mechanical Saw


### Outputs
- 1x Andesite Casing

### Workflow Diagram

```mermaid
flowchart TD
	Log[Log]
	StrippedLog[Stripped Log]
	Casing[Andesite Casing]
	Saw(Mechanical Saw)
	Deployer(Deployer: Andesite Alloy)
	
	Log --> | 1x | Saw
	Saw --> | 1x | StrippedLog
	StrippedLog --> | 1x | Deployer
	Deployer --> | 1x | Casing
```
