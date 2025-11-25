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
* `wealth SubclassOf canAfford some healthcare` <br />
natural language description
