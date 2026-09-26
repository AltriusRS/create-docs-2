---
tags:
  - recipes
  - recipes/items
  - inputs/gold_ingot
  - inputs/small_cogwheel
  - inputs/large_cogwheel
  - inputs/iron_nugget
  - outputs/precision_mechanism
  - outputs/random_salvage
---

### Inputs
- 1x Gold Ingot
- 5x [[Small Cogwheel]]
- 5x [[Large Cogwheel]]
- 5x Iron Nugget

### Requires
- Deployer
- Mechanical Press

### Outputs
- 80% chance - 1x Precision Mechanism
- 20% chance - "random salvage"


```mermaid
flowchart TD
	GoldIngot[Gold Ingot]
	GoldPlate[Gold Plate]
	PrecisionMechanism[Precision Mechanism]
	Salvage[Random Salvage]
	DeploySC(Deployer: Small Cogwheel)
	DeployLC(Deployer: Large Cogwheel)
	DeployIN(Deployer: Iron Nugget)
	Press(Mechanical Press)
	
	GoldIngot --> | 1x | Press
	Press --> | 1x | GoldPlate
	GoldPlate --> | 1x Small Cogwheel | DeploySC
	DeploySC --> DeployLC
	DeployLC --> DeployIN
	DeployIN --> | Repeat 5x | DeploySC 
	DeployIN --> | 80% chance | PrecisionMechanism
	DeployIN --> | 20% chance | Salvage
```