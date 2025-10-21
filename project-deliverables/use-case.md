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
  * 
* [Hospital Registration Information](https://data.ohio.gov/wps/portal/gov/data/view/hospital-registration-information)
  * 
* [Infant Mortality Scorecard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-infant-mortality-scorecard)
  * 
* [Mortality](https://data.ohio.gov/wps/portal/gov/data/view/mortality)
  * 
* [National DPP Locator Map](https://data.ohio.gov/wps/portal/gov/data/view/national-diabetes-prevention-program-_national-dpp_-locator-map)
  *
* [ODH Respiratory Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-department-of-health-respiratory-dashboard)
  *
* [Ohio BRFSS Annual Report](https://data.ohio.gov/wps/portal/gov/data/view/ohio-brfss-annual-report)
  *
* [Ohio BRFSS Data](https://data.ohio.gov/wps/portal/gov/data/view/ohio-brfss-data)
  *
* [Ohio Pharmacy Access](https://data.ohio.gov/wps/portal/gov/data/view/ohio-pharmacy-assessment-)
  *
* [Population Data for Calculating Rates](https://data.ohio.gov/wps/portal/gov/data/view/population-data-for-calculating-rates)
  *
* [Summary of Infectious Diseases in Ohio](https://data.ohio.gov/wps/portal/gov/data/view/summary-of-infectious-diseases-in-ohio)
  *
* [Tobacco Use with Referral Info](https://data.ohio.gov/wps/portal/gov/data/view/tobacco-use-with-referral-info)
  * 

## References

[0]  National Institute of Environmental Health Sciences, “Air pollution and your health,” National Institute of Environmental Health Sciences, Aug. 06, 2024. https://www.niehs.nih.gov/health/topics/agents/air-pollution

[1]  R. D. Guzman and J. Schiller, “Air pollution and its impact on cancer incidence, cancer care and cancer outcomes,” BMJ Oncology, vol. 4, no. 1, pp. e000535–e000535, Mar. 2025, doi: https://doi.org/10.1136/bmjonc-2024-000535.

[2]  National Sleep Foundation, “What is sleep quality?,” National Sleep Foundation, Apr. 12, 2024. https://www.thensf.org/what-is-sleep-quality/
