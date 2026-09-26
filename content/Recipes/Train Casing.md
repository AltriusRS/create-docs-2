---
tags:
  - recipes
  - recipes/casings
  - inputs/brass_casing
  - inputs/sturdy_sheet
  - outputs/train_casing
---

### Inputs
- 1x [[Brass Casing]]
- 1x Sturdy Sheet

### Requires
- Deployer


### Outputs
- 1x Train Casing


```mermaid
flowchart TD
	Casing[Brass Casing]
	Saw(Mechanical Saw)
	Deployer(Deployer: Sturdy Sheet)
	
	Log --> | 1x | Saw
	Saw --> | 1x | StrippedLog
	StrippedLog --> | 1x | Deployer
	Deployer --> | 1x | Casing
```
