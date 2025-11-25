# Factorizing Determinants of Human Health

![all-schemas](schema-diagrams)

## Education Module
![schema-diagram](schema-diagrams/education.jpg)

### Axioms
* `EducationLevel subClassOf Education` <br />
If there is Education, there is an Education Level descriptor.
* `EducationLevel subClassOf Education some Income.` <br />
If there is some EducationLevel, it is usually a large influence on Income level.

## Environment Module
![schema-diagram](schema-diagrams/environment.jpg)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## HealthcareAccess Module
![schema-diagram](schema-diagrams/PharmacyAccess.jpg)

### Axioms
* `HospitalAccess subClassOf HealthcareAccess` <br />
HospitalAccess is a component of HealthcareAccess.
* `PharmacyAccess subClassOf HealthcareAccess` <br />
PharmacyAccess is a component of HealthcareAccess.
* `Pharmacyaccess DisjointWith hospitalaccess` <br />
A Hospital oftentimes contains its own Pharmacy, but its Pharmacy is generally only used by immediate patients. PharmacyAccess data refers to Pharmacy locations not attached to a Hospital.
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
![schema-diagram](schema-diagrams/keyBehaviors.jpg)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## Life Module
![schema-diagram](schema-diagrams/LifeModule.jpg)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## LifeEvent Module
![schema-diagram](schema-diagrams/lifeEvent.jpg)

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

## Person
![schema-diagram](schema-diagrams/person.jpg)

### Axioms
* `IndividualHuman SubclassOf Person max 1 Lifespan` <br />
natural language description
* `IndividualHuman subclassOf Person some RacialAttribute` <br />
If an IndividualHuman exists, that IndividualHuman has some RacialAttribute.
* `IndividualHuman SubclassOf Person max 1 EducationLevel` <br />
If an IndividualHuman exists, that IndividualHuman has at most one generally-quantifiable EducationLevel.
* `IndividualHuman SubclassOf Person max 1 Income` <br />
natural language description

## Population Module
![schema-diagram](schema-diagrams/PopulationModule.jpg)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

## RacialAttribute Module
![schema-diagram](schema-diagrams/raceAttribute.jpg)

### Axioms
* `GeneticPredisposition subClassOf RacialAttribute some Condition` <br />
If a RacialAttribute includes a given GeneticPredispostion, there are corresponding medical Conditons that are more likely.
* `GeneticPredisposition subClassOf RacialAttribute some HealthOutcome` <br />
If a RacialAttribute includes a given GeneticPredispostion, there are corresponding HealthOutcomes that could arise from the predisposed Conditions.

## Wealth
![schema-diagram](schema-diagrams/WealthModule.jpg)

### Axioms
* `Currency subclassOf Income some Value` <br />
If Currency is a type of Income, it has some quantifiable monetary Value.
* `Income subclassOf WealthModule some Healthcare` <br />
If Wealth exists, some level of Healthcare can be afforded.
* `Income subClassOf WealthModule some EducationLevel.` <br />
If a Person has some Income, it enables that Person to obtain some EducationLevel.