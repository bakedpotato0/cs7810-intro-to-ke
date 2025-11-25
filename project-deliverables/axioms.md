# Factorizing Determinants of Human Health

![all-schemas](schema-diagrams)

## Education Module
![schema-diagram](schema-diagrams/education.jpg)

### Axioms
* `EducationLevel subClassOf Education` <br />
If there is Education, there is an EducationLevel descriptor.
* `EducationLevel subClassOf Education some Income.` <br />
If there is some EducationLevel, it is usually an influence on Income level.

## Environment Module
![schema-diagram](schema-diagrams/environment.jpg)

### Axioms
* `Environment some describable PollutionType` <br />
If an Environment exists, it must have some description of its PollutionType (including "clean"/"sterile").
* `Environment some HealthOutcome` <br />
If an Environment exists, it may influence the chance of certain HealthOutcomes.

## HealthcareAccess Module
![schema-diagram](schema-diagrams/PharmacyAccess.jpg)

### Axioms
* `HospitalAccess subClassOf HealthcareAccess` <br />
HospitalAccess is a component of HealthcareAccess.
* `PharmacyAccess subClassOf HealthcareAccess` <br />
PharmacyAccess is a component of HealthcareAccess.
* `Pharmacyaccess DisjointWith HospitalAccess` <br />
A Hospital oftentimes contains its own Pharmacy, but the concern of PharmacyAccess is to supply an IndividualHuman with medication for treating a Condition outside of a Hospital setting.
* `HealthcareAccess subClassOf HealthcareAccess Module some Healthcare` <br />
If there is HealthcareAccess, then there is some level of Healthcare accessible.
* `EndingFix subClassOf HealthcareAccess Module some HealthOutcome` <br />
If there is an EndingFix, there is some (positive or negative) influence on a HealthOutcome.

## HealthOutcomes Module
![schema-diagram](schema-diagrams/HealthOutcomeModule.jpg)

### Axioms
* `HealthOutcome subClassOf LifeEvent some Cost` <br />
A HealthOutcome is a type of LifeEvent that has some Cost and influences further LifeEvents.
* `HealthOutcome subClassOf LifeEvent some startingCondition` <br />
If there is a HealthOutcome then there is a startingCondition with descriptor conditionDescription.
* `HealthOutcome subClassOf LifeEvent some endingCondition` <br />
If there is a HealthOutcome then there is an endingCondition with descriptor conditionDescription.

## KeyBehaviors Module
![schema-diagram](schema-diagrams/keyBehaviors.jpg)

### Axioms
* `Action subClassOf KeyBehaviors some description` <br />
If an Action exists, it must have some description.
* `Action subClassOf KeyBehaviors some HealthOutcome` <br />
If an Action exists, it must have some influence on some HealthOutcome.

## Life Module
![schema-diagram](schema-diagrams/LifeModule.jpg)

### Axioms
* `LifeSpan subClassOf Life some measureOfTime` <br />
If a LifeSpan exists, its length of Time can be measured.

## LifeEvent Module
![schema-diagram](schema-diagrams/lifeEvent.jpg)

### Axioms
* `LifeEvent subClassOf RecurrentEvent some LifeEvent` <br />
LifeEvents lead to more LifeEvents until the cycle reaches EventualDeath.
* `EventualDeath subClassOf LifeEvent max 1 LifeSpan` <br />
If LifeEvents occur, there will be an EventualDeath which is the ending point of an IndividualHuman's LifeSpan.

## Location Module
![schema-diagram](relative/path/to/schema/diagram)

### Axioms
* `Location some HealthcareAccess` <br />
If some Location exists, it has some influence on HealthcareAccess services, including distance to Hospitals, Pharmacies, and other Healthcare services.

## Person
![schema-diagram](schema-diagrams/person.jpg)

### Axioms
* `IndividualHuman subClassOf Person max 1 LifeSpan` <br />
If an IndividualHuman exists, that IndividualHuman has at most one LifeSpan.
* `IndividualHuman subClassOf Person some RacialAttribute` <br />
If an IndividualHuman exists, that IndividualHuman has some RacialAttribute.
* `IndividualHuman subClassOf Person max 1 EducationLevel` <br />
If an IndividualHuman exists, that IndividualHuman has at most one generally-quantifiable EducationLevel.
* `IndividualHuman subClassOf Person max 1 Income` <br />
If an IndividualHuman exists, that IndividualHuman has at most one total quantifiable Income.
* `IndividualHuman subClassOf Person max 1 alias` <br />
If an IndividualHuman exists, that IndividualHuman has at most one alias in the data. This alias must be kept anonymized in the model for privacy and security reasons.
* `IndividualHuman subClassOf Person some Condition` <br />
If an IndividualHuman exists, that IndividualHuman has some describable Condition (healthy, ill, etc.).
* `IndividualHuman subClassOf Person some Environment` <br />
If an IndividualHuman exists, that IndividualHuman must inhabit some describable Environment, and may work in the same or a different Environment.
* `IndividualHuman subClassOf Person some Population` <br />
If an IndividualHuman exists, that IndividualHuman is a member of some Population.
* `IndividualHuman subClassOf Person some Action` <br />
If an IndividualHuman exists, that IndividualHuman performs some Action.

## Population Module
![schema-diagram](schema-diagrams/PopulationModule.jpg)

### Axioms
* `Population some Location` <br />
If a Population exists, it must have some describable Location.
* `PublicWelfare subClassOf Population some Condition` <br />
If a Population exists, it must have some description of its PublicWelfare.

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
* `Currency subClassOf Income some Value` <br />
If Currency is a type of Income, it has some quantifiable monetary Value.
* `Income subClassOf WealthModule some Healthcare` <br />
If Wealth exists, some level of Healthcare can be afforded.
* `Income subClassOf WealthModule some EducationLevel.` <br />
If a Person has some Income, it enables that Person to obtain some EducationLevel.