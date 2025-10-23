# Use Case
## Narrative
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


## Competency Questions
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

## Potential Datasets
* [Behavioral Health Claims Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/mental-health-and-addiction-services-claims-dashboard)
   *
* [Blood Lead Testing Public](https://data.ohio.gov/wps/portal/gov/data/view/blood-lead-testing-public-_2016-present_)
   *
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
   * number of deaths
* [National DPP Locator Map](https://data.ohio.gov/wps/portal/gov/data/view/national-diabetes-prevention-program-_national-dpp_-locator-map)
   * county
* [ODH Respiratory Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-department-of-health-respiratory-dashboard)
   *
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
   *
* [Population Data for Calculating Rates](https://data.ohio.gov/wps/portal/gov/data/view/population-data-for-calculating-rates)
   *
* [Summary of Infectious Diseases in Ohio](https://data.ohio.gov/wps/portal/gov/data/view/summary-of-infectious-diseases-in-ohio)
   * reportable condition
   * county
* [Tobacco Use with Referral Info](https://data.ohio.gov/wps/portal/gov/data/view/tobacco-use-with-referral-info)
   * age
   * sex
   * county
   *


## References

[0]  National Institute of Environmental Health Sciences, “Air pollution and your health,” National Institute of Environmental Health Sciences, Aug. 06, 2024. https://www.niehs.nih.gov/health/topics/agents/air-pollution

[1]  R. D. Guzman and J. Schiller, “Air pollution and its impact on cancer incidence, cancer care and cancer outcomes,” BMJ Oncology, vol. 4, no. 1, pp. e000535–e000535, Mar. 2025, doi: https://doi.org/10.1136/bmjonc-2024-000535.

[2]  National Sleep Foundation, “What is sleep quality?,” National Sleep Foundation, Apr. 12, 2024. https://www.thensf.org/what-is-sleep-quality/



