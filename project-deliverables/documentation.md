# Create Documentation
This deliverable has two components: the documentation file and the presentation.

## Documentation
1. Create a file named `documentation.md` using the [template](../templates/documentation.md) and place it in the `deliverables` directory.
2. Adapt the sections from the previous project deliverables. There is additional guidance in the template.
    * The modules section should have one section per module (i.e., effectively each key notion).
    * The overview section should contain the overall schema diagram.

## Presentation
1. Create a presentation version of the documentation file.
    * Consider using [marp](https://marp.app/).
3. Add an additional section at the end called "Retrospective".
    * In this section, put 1-2 comments per group member
    * Include comments re: what went well in this course, what could be changed
    * Provide an overall rating for the course: fun/!fun, useful/!useful, etc.
4. Upload a PDF rendering of the presentation to the `deliverables` directory.

**Note:** Ensure that each member contributes in explicit commits. Do not squash commits; the `git` history will serve as a record of participation and contribution.


# Factorizing Determinants of Human Health
**Authors:** Nicholas Latham, Chris Nodel, Van Quoc Huy Vo

## Use Case Scenario
### Narrative 
Life expectancy is a measure that reflects the average number of years that a human is expected to live based on a variety of diverse factors. Generally, life expectancy is used to judge the average health of a society.
In addition to genetic predispositions, life expectancy is greatly influenced by a combination of environmental, social, and behavioral influences.
Across the state of Ohio, as in many parts of the United States, significant disparities in life expectancy may exist between different counties, ZIP codes, and even neighborhoods.
This presents an opportunity to better understand and address the root causes of these variations through a data-driven approach.

Our primary objective is to develop a knowledge graph model that estimates life expectancy for residents of all Ohio counties by integrating a wide range of datasets.
Using a knowledge graph will allow us to view and compare different segments of the Ohio population and more easily understand their average health.
Our knowledge graph could conceivably be used to aid healthcare experts, guide government policies, and increase public awareness of both health risks and beneficial factors.
The model will incorporate environmental data such as water quality and pollution.
These environmental exposures have been directly linked to serious medical issues, such as respiratory issues [0] and various forms of cancer [1], and all of which negatively affect longevity.

Behavioral factors influencing life expectancy include:
* Physical Activity: Engaging in regular moderate to vigorous physical activity can significantly increase life expectancy and reduce mortality risk. 
* Healthy Diet: A healthy, balanced diet is linked to better survival rates and can contribute to a longer, healthier life. 
* Smoking: Avoiding smoking and quitting the habit can improve life expectancy and reduce the risk of death from smoking-related diseases. 
* Alcohol Consumption: Moderate alcohol consumption is part of a healthy lifestyle, with heavy or irregular drinking being detrimental to life expectancy. 
* Sleep Quality: Maintaining a healthy sleep routine, such as sleeping 7–8 hours a day, is associated with greater survival chances. [2]


Social factors influencing life expectancy include:
* Having a strong social support systems is associated with better health outcomes and longer life
* Higher level of education also associated with longer life expectancy
* Higher or lower income are correlated with longer lifespans
* Community resources: good job, quality healthcare or nutritious food can improve health and extend life

We have located several pertinent datasets from DataOhio, an Ohio state government website.
In addition to the factors listed above, we also have found datasets regarding mental health issues, pharmacy access, communicable respiratory illness cases, diabetes, and mortality information.
We are also looking to expand our dataset collection with sets from the National Library of Medicine’s National Center for Biotechnology Information and the National Cancer Institute’s Cancer Research Data Commons- both maintained by the U.S. Federal government through the National Institutes of Health.

Our ultimate goal is to create a scalable knowledge graph which can be used to inform policymakers, healthcare providers, community organizations, and the general public. As more data is added, a more nuanced understanding of public health can be achieved.

### Competency Questions
*How do lead levels affect life expectancy?<br>
Bridges Datasets: Blood Lead Levels, Mortality
* Is RSV more dangerous to adults than infants?<br>
Bridges Datasets: ODH Respiratory Dashboard, Mortality, Infant Mortality
* Is secondhand smoke more dangerous than vaping?<br>
Bridges Datasets: eCigarette Use, Tobacco Use, Mortality
* Does pharmacy access improve mental health outcomes?<br>
Bridges Datasets: Pharmacy Access, Behavioral Health Claims Dashboard
* Do diabetes prevention programs decrease diabetes-related hospitalizations?<br>
Bridges Datasets: National DPP Locator Map, Hospital Registration Information
* What infectious diseases correlate to higher infant mortality?<br>
Bridges Datasets: Summary of Infectious Diseases, Infant Mortality
* Do tobacco and eCigarette usage increase risk of dying from an infectious respiratory illness?<br>
Bridges Datasets: Tobacco Use, eCigarette Use, ODH Respiratory Dashboard, Mortality
* Does lead exposure increase mental health claims?<br>
Bridges Datasets: Blood Lead Testing, Behavioral Health Claims
* How much does lead exposure increase infant mortality?<br>
Bridges Datasets: Blood Lead Testing, Infant Mortality
* How does cardiovascular disease correlate with mental health issues?<br>
Bridges Datasets: Behavioral Health Claims, BRFSS Annual Report

### Integrated Datasets
* [Behavioral Health Claims Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/mental-health-and-addiction-services-claims-dashboard)
   * age group
   * gender
   * race
   * ethnicity
   * current county of residence
   * current county of residence type
   * current board name
   * hospital catchment
   * primary diagnosis type
* [Best Hospitals in Ohio](https://health.usnews.com/best-hospitals/area/oh)
   * National Ohio Rankings
   * Specialties
   * Children's Specialties
   * Procedures/Conditions
   * location
* [Blood Lead Testing Public](https://data.ohio.gov/wps/portal/gov/data/view/blood-lead-testing-public-_2016-present_)
   * year
   * age group
   * blood-lead micrograms/deciliter
* [Cancer Data and Statistics](https://www.cdc.gov/cancer/data/index.html)
   * location (state)
   * date (year)
   * Rate of New Cancers
   * Rate of Cancer Deaths
   * Cancer Site
* [eCigarette Use with Referral Info](https://data.ohio.gov/wps/portal/gov/data/view/ecigarette-use-with-referral-info)
   * age
   * sex
   * county
   * ethnicity
* [Hospital Registration Information](https://data.ohio.gov/wps/portal/gov/data/view/hospital-registration-information)
   * report year
   * hospital dba name
   * hospital number
   * address
   * city
   * state
   * zip code
   * county
   * medicare name
   * corporate phone
   * national provider identifier
   * medicare provider number
   * business entity type
   * type_of_organization_responsible_for_overall_operational_polic
   * hospital_part_of_a_multi_hospital_system
   * system name
   * medicare classification
   * category_best_describing_hospital_services
   * other_service_category
   * joint_commission_accreditation
   * hfap_accreditation
   * medicare_certified
   * dnv_accreditation
   * date_of_last_accreditation_survey
   * date_of_last_certification_survey
   * distinct_part_psych_unit
   * distinct_part_rehab_unit
   * transplant_center
   * maternity_unit
   * medical_and_surgical_service_type
   * surgical_cases_inpatient
   * surgical_cases_outpatient
   * number_surgical_operating_rooms_inpatient
   * number_surgical_operating_rooms_outpatient
   * number_surgical_services_dual_purpose_operating_rooms
   * total_operating_rooms_onsite
   * total_operating_rooms_offsite
   * emergency_services_type
   * emergency_services_treated_and_admitted
   * emergency_services_treated_and_released
   * trauma_level_adult
   * trauma_level_pediatric
   * cardiac_service_type
   * adult_cardiac_catheterizations
   * pediatric_cardiac_catheterizations
   * adult_open_heart_procedures
   * pediatric_cardiovascular_procedures
   * obstetric_level
   * newborn_level
   * beds_category
   * number_of_admissions_for_beds_category
   * patient_days
   * beds_in_use
   * registered_beds
   * occupancy_rate
   * average_length_of_stay
   * discharged_to_home_without_referral_to_home_care_or_hospice
   * discharged_to_home_with_referral_to_home_care
   * discharged_to_home_with_referral_to_hospice
   * discharged_to_inpatient_service_of_a_hospice_care_program
   * tranfers_to_other_hospitals
   * transfers_to_a_nursing_home
   * expired
   * total_discharges
   * registration_status
   * query_run_date
* [Infant Mortality Scorecard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-infant-mortality-scorecard)
   * county
   * ethnicity
   * age category
   * birth outcomes
	  * preterm birth
	  * extreme preterm
	  * low birth weight
	  * extreme low birth weight
   * maternal characteristics
	  * smoker
	  * prenatal care received
	  * adequacy of prenatal care
	  * obese weight pre-pregnancy
	  * breastfed at discharge
	  * appropriate pregnancy weight
	  * interpregnancy interval under 18 months
* [Mortality](https://data.ohio.gov/wps/portal/gov/data/view/mortality)
   * county
   * year
   * death count
* [National DPP Locator Map](https://data.ohio.gov/wps/portal/gov/data/view/national-diabetes-prevention-program-_national-dpp_-locator-map)
   * name
   * address
   * city
   * state
   * zip
   * contact
   * website
   * email
   * phone
* [ODH Respiratory Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-department-of-health-respiratory-dashboard)
   * age
   * county
   * district
   * week
   * hospitalized
   * covid19
   * flu
   * rsv
* [Ohio BRFSS Annual Report](https://data.ohio.gov/wps/portal/gov/data/view/ohio-brfss-annual-report)
   * condition
   * ethnicity
   * sex
   * age
   * education level
   * percent affected
   * region
   *
* [Ohio BRFSS Data](https://data.ohio.gov/wps/portal/gov/data/view/ohio-brfss-data)
   * condition
   * ethnicity
   * sex
   * age
   * education level
   * percent affected
   * region
   *
* [Ohio Pharmacy Access](https://data.ohio.gov/wps/portal/gov/data/view/ohio-pharmacy-assessment-)
   * name
   * location
   * open_date
   * closed_date
   * pharmacy_type
* [Population Data for Calculating Rates](https://data.ohio.gov/wps/portal/gov/data/view/population-data-for-calculating-rates)
   * year
   * countyCD
   * age
   * raceCD
   * sexCD
   * hispanicCD
   * count
   * AgeCDMCH
   * AgeCDNCHS
   * AgeCDNCI
   * AgeCDSTD
   * AgeBirth
   * PopulationID
   * AgeCDODRS
   * AgeCDEHARS
* [Summary of Infectious Diseases in Ohio](https://data.ohio.gov/wps/portal/gov/data/view/summary-of-infectious-diseases-in-ohio)
   * reportable condition
   * county
   * report start date
   * report end date
* [Tobacco Use with Referral Info](https://data.ohio.gov/wps/portal/gov/data/view/tobacco-use-with-referral-info)
   * age
   * sex
   * county
   * tobacco_type

### References
[0]  National Institute of Environmental Health Sciences, “Air pollution and your health,” National Institute of Environmental Health Sciences, Aug. 06, 2024. https://www.niehs.nih.gov/health/topics/agents/air-pollution

[1]  R. D. Guzman and J. Schiller, “Air pollution and its impact on cancer incidence, cancer care and cancer outcomes,” BMJ Oncology, vol. 4, no. 1, pp. e000535–e000535, Mar. 2025, doi: https://doi.org/10.1136/bmjonc-2024-000535.

[2]  National Sleep Foundation, “What is sleep quality?,” National Sleep Foundation, Apr. 12, 2024. https://www.thensf.org/what-is-sleep-quality/

## Modules
<!-- There should be one module section per module (essentially per key-notion) -->
### Module X
**Source Pattern:** name of adapted source pattern
**Source Data:** name(s) of dataset(s) which populate this module

#### Description
Description Text (adapted from the rationale in `key-notions.md`).

![schema-diagram](./schema-diagram.png)

#### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

#### Remarks
* Any remarks re: usage

### Education Module
**Source Pattern:** name of adapted source pattern
**Source Data:** name(s) of dataset(s) which populate this module

#### Description
Description Text (adapted from the rationale in `key-notions.md`).

![schema-diagram](schema-diagrams/education.jpg)

#### Axioms
* `EducationLevel subClassOf Education` <br />
If there is Education, there is an EducationLevel descriptor.
* `EducationLevel subClassOf Education some Income.` <br />
If there is some EducationLevel, it is usually an influence on Income level.

#### Remarks
* Any remarks re: usage

### Environment Module
**Source Pattern:** name of adapted source pattern
**Source Data:** name(s) of dataset(s) which populate this module

#### Description
Description Text (adapted from the rationale in `key-notions.md`).

![schema-diagram](schema-diagrams/environment.jpg)

#### Axioms
* `Environment subClassOf Environment Module some PollutionType` <br />
If an Environment exists, it must have some description of its PollutionType (including "clean"/"sterile").
* `Environment subClassOf Environment Module some HealthOutcome` <br />
If an Environment exists, it may influence the chance of certain HealthOutcomes.

#### Remarks
* Any remarks re: usage

### HealthcareAccess Module
**Source Pattern:** name of adapted source pattern
**Source Data:** name(s) of dataset(s) which populate this module

#### Description
Description Text (adapted from the rationale in `key-notions.md`).

![schema-diagram](schema-diagrams/Healthcare%20Access.jpg)

#### Axioms
* `HospitalAccess subClassOf HealthcareAccess` <br />
HospitalAccess is a component of HealthcareAccess.
* `PharmacyAccess subClassOf HealthcareAccess` <br />
PharmacyAccess is a component of HealthcareAccess.
* `Pharmacyaccess DisjointWith HospitalAccess` <br />
A Hospital oftentimes contains its own Pharmacy, but the concern of PharmacyAccess is to supply an IndividualHuman with medication for treating a Condition outside of a Hospital setting.
* `HealthcareAccess subClassOf HealthcareAccess Module some Healthcare` <br />
If there is HealthcareAccess, then there is some level of Healthcare service accessible.
* `EndingFix subClassOf HealthcareAccess Module some HealthOutcome` <br />
If there is an EndingFix, there is some (positive or negative) influence on the chance of a HealthOutcome.

#### Remarks
* Any remarks re: usage

### HealthOutcomes Module
**Source Pattern:** name of adapted source pattern
**Source Data:** name(s) of dataset(s) which populate this module

#### Description
Description Text (adapted from the rationale in `key-notions.md`).

![schema-diagram](schema-diagrams/HealthOutcomeModule.jpg)

#### Axioms
* `HealthOutcome subClassOf LifeEvent some Cost` <br />
A HealthOutcome is a type of LifeEvent that has some Cost and influences further LifeEvents.
* `HealthOutcome subClassOf LifeEvent some startingCondition` <br />
If there is a HealthOutcome, then there is a startingCondition with descriptor conditionDescription.
* `HealthOutcome subClassOf LifeEvent some endingCondition` <br />
If there is a HealthOutcome, then there is an endingCondition with descriptor conditionDescription.

#### Remarks
* Any remarks re: usage
- modify from here down
## KeyBehaviors Module
![schema-diagram](schema-diagrams/keyBehaviors.jpg)

### Axioms
* `Action subClassOf KeyBehaviors some description` <br />
If an Action exists, it must have some description.
* `Action subClassOf KeyBehaviors some HealthOutcome` <br />
If an Action exists, it must have some influence on some HealthOutcome.

### Life Module
![schema-diagram](schema-diagrams/LifeModule.jpg)

#### Axioms
* `LifeSpan subClassOf Life some measureOfTime` <br />
If a LifeSpan exists, its length of Time can be measured.

### LifeEvent Module
![schema-diagram](schema-diagrams/lifeEvent.jpg)

#### Axioms
* `LifeEvent subClassOf RecurrentEvent some LifeEvent` <br />
LifeEvents lead to more LifeEvents, until the cycle reaches EventualDeath.
* `EventualDeath subClassOf LifeEvent max 1 LifeSpan` <br />
If LifeEvents occur, there will be an EventualDeath which is the ending point of an IndividualHuman's LifeSpan.

### Location Module
![schema-diagram](relative/path/to/schema/diagram)

#### Axioms
* `Location subClassOf Location Module some HealthcareAccess` <br />
If some Location exists, it has some influence on HealthcareAccess services, including proximity to Hospitals, Pharmacies, and other Healthcare services.

### Person Module
![schema-diagram](schema-diagrams/person.jpg)

#### Axioms
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
If an IndividualHuman exists, that IndividualHuman has some describable Condition ("healthy," "ill," or something more detailed).
* `IndividualHuman subClassOf Person some Environment` <br />
If an IndividualHuman exists, that IndividualHuman must inhabit some describable Environment, and may work a job in the same or a different Environment.
* `IndividualHuman subClassOf Person some Population` <br />
If an IndividualHuman exists, that IndividualHuman is a member of some Population.
* `IndividualHuman subClassOf Person some Action` <br />
If an IndividualHuman exists, that IndividualHuman performs some Action.
* `IndividualHuman subClassOf Person some HealthOutcome` <br />
If an IndividualHuman exists, that IndividualHuman has some HealthOutcomes during their LifeSpan.

### Population Module
![schema-diagram](schema-diagrams/PopulationModule.jpg)

#### Axioms
* `Population subClassOf Population Module some Location` <br />
If a Population exists, it must have some describable Location.
* `Population subClassOf Population Module some populationCount` <br />
If a Population exists, it must have some countable number of members.
* `PublicWelfare subClassOf Population some Condition` <br />
If a Population exists, it must have some description of its PublicWelfare.

### RacialAttribute Module
![schema-diagram](schema-diagrams/raceAttribute.jpg)

#### Axioms
* `GeneticPredisposition subClassOf RacialAttribute some Condition` <br />
If a RacialAttribute includes a given GeneticPredispostion, there are corresponding medical Conditons that are more likely.
* `GeneticPredisposition subClassOf RacialAttribute some HealthOutcome` <br />
If a RacialAttribute includes a given GeneticPredispostion, there are corresponding HealthOutcomes that could arise from the predisposed Conditions.

### Wealth
![schema-diagram](schema-diagrams/WealthModule.jpg)

#### Axioms
* `Currency subClassOf Income some Value` <br />
If Currency is a type of Income, it has some quantifiable monetary Value.
* `Income subClassOf WealthModule some HealthcareAccess` <br />
If Wealth exists, some level of HealthcareAccess can be afforded.
* `Income subClassOf WealthModule some EducationLevel.` <br />
If a Person has some Income, it enables that Person to obtain some EducationLevel.
- modify from here up

## The Overall Knowledge Graph
### Namespaces
* prefix: namespace
* prefix: namespace

### Schema Diagram
![schema-diagram](./schema-diagram.png)

### Axioms
* `axiom in manchester syntax` <br />
natural language description
* `axiom in manchester syntax` <br />
natural language description

### Usage
Adapted from `validation.md`, i.e., the competency questions + SPARQL queries.

## Retrospective
* In this section, put 1-2 comments per group member
* Include comments re: what went well in this course, what could be changed
* Provide an overall rating for the course: fun/!fun, useful/!useful, etc.