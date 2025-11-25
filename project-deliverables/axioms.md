# Name of Ontology

![all-schemas](schema-diagrams)

## Education Module
![schema-diagram](schema-diagrams/education.jpg)

### Axioms
* `EducationLevel subClassOf Education` <br />
If there is Education, there is an Education Level descriptor.


## HealthcareAccess Module
![schema-diagram](schema-diagrams/PharmacyAccess.jpg)

### Axioms
* `HospitalAccess subClassOf HealthcareAccess` <br />
HospitalAccess is a component of HealthcareAccess.
* `PharmacyAccess subClassOf HealthcareAccess` <br />
PharmacyAccess is a component of HealthcareAccess.
* `HealthcareAccess subClassOf HealthcareAccess Module some Healthcare` <br />
If there is HealthcareAccess, then there is some level of Healthcare accessible.
* `EndingFix subClassOf HealthcareAccess Module some HealthOutcome` <br />
If there is an EndingFix, there is some (positive or negative) influence on a HealthOutcome.

## HealthOutcomes Module
![schema-diagram](schema-diagrams/HealthOutcomeModule.jpg)

### Axioms
* `HealthOutcome subClassOf LifeEvent some Cost` <br />
A HealthOutcome is a type of LifeEvent that has some Cost.
* `HealthOutcome subClassOf LifeEvent some startingCondition` <br />
If there is a HealthOutcome then there is a startingCondition with descriptor conditionDescription.
* `HealthOutcome subClassOf LifeEvent some endingCondition` <br />
If there is a HealthOutcome then there is an endingCondition with descriptor conditionDescription.

## KeyBehaviors Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Life Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## LifeEvent Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Location Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Person Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Population Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## RacialAttribute Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Wealth Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Name of Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description
