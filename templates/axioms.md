# Name of Ontology

![all-schemas](relative/path/to/all/schemas)

## HealthcareAccess
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `pharmacyaccess SubclassOf healthcareaccess` <br />
natural language description
* `hospitalaccess SubclassOf healthcareaccess` <br />
natural language description
* `pharmacyaccess DisjointWith hospitalaccess` <br />
natural language description
* `healthcareaccess SubclassOf includes max 1 healthcare` <br />
natural language description

## Wealth
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `income SubclassOf hasValue only currency` <br />
natural language description
* `wealth SubclassOf canAfford some healthcareaccess` <br />
natural language description

## Person
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `person SubclassOf hasOne lifespan` <br />
natural language description
* `peson SubclassOf has some racialattribute` <br />
natural language description
* `peson SubclassOf hasOne max 1 educationlevel` <br />
natural language description
* `peson SubclassOf hasOne max 1 income` <br />
natural language description
* `peson SubclassOf performs only keybehaviors` <br />
natural language description
* `madeof some popuiation SubclassOf person` <br />
natural language description
