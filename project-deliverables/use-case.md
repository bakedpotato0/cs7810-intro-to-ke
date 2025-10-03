# Build the Use-case
1. Create a file called `use-case.md` from the [template](../templates/use-case.md).
2. Fill the `Narrative` section with a top-level description of your use-case, including references. As a guideline, this section should be about 500 words. This should, at a minimum, answer the questions:
    * Who are you supporting?
    * What are their goals?
    * Why is making a Knowledge Graph interesting -- or important -- for the use-case? 
    * Why a knowledge graph and not a relational (tabular) database?
3. Fill the `Competency Questions` section with no fewer than 10 competency questions. Thoroughly describe your intended interactions and what data will be retrieved to support said interactions.
4. Fill the `Potential Datasets` section with links and access dates for no less than five potential datasets.
5. Fill the `Existing Resources` section with any resources (e.g., ontologies, knowledge graphs, or standards) which can be used in the project.
6. Provide all references in the `References` section. References should be numbered starting at 1, listed in order of appearance, and otherwise following the IEEE reference style. Ensure that the DOI is included for every reference, where available.

**Note:** Ensure that each member contributes in explicit commits. Do not squash commits; the `git` history will serve as a record of participation and contribution.

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
These environmental exposures have been directly linked to serious medical issues, such as respiratory issues and various forms of cancer, and all of which negatively affect longevity.

Behavioral factors influencing life expectancy include:
* Physical Activity: Engaging in regular moderate to vigorous physical activity can significantly increase life expectancy and reduce mortality risk. 
* Healthy Diet: A healthy, balanced diet is linked to better survival rates and can contribute to a longer, healthier life. 
* Smoking: Avoiding smoking and quitting the habit can improve life expectancy and reduce the risk of death from smoking-related diseases. 
* Alcohol Consumption: Moderate alcohol consumption is part of a healthy lifestyle, with heavy or irregular drinking being detrimental to life expectancy. 
* Sleep Quality: Maintaining a healthy sleep routine, such as sleeping 7–8 hours a day, is associated with greater survival chances.

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
* Competency Question<br>
Bridges Datasets: dataset 1, dataset 2, ...
* Competency Question<br>
Bridges Datasets: dataset 1, dataset 2, ...
* Competency Question<br>
Bridges Datasets: dataset 1, dataset 2, …
* Competency Question<br>
Bridges Datasets: dataset 1, dataset 2, ...

## Potential Datasets
* [National Diabetes Prevention Program (National DPP) Locator Map](https://data.ohio.gov/wps/portal/gov/data/view/national-diabetes-prevention-program-_national-dpp_-locator-map)
* [Summary of Infectious Diseases in Ohio](https://data.ohio.gov/wps/portal/gov/data/view/summary-of-infectious-diseases-in-ohio)
* [ODH Respiratory Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-department-of-health-respiratory-dashboard)
* [Mortality](https://data.ohio.gov/wps/portal/gov/data/view/mortality)
* [Infant Mortality Scorecard](https://data.ohio.gov/wps/portal/gov/data/view/ohio-infant-mortality-scorecard)
* [Behavioral Health Claims Dashboard](https://data.ohio.gov/wps/portal/gov/data/view/mental-health-and-addiction-services-claims-dashboard)
* [eCigarette Use with Referral Info](https://data.ohio.gov/wps/portal/gov/data/view/ecigarette-use-with-referral-info)
* [Ohio Pharmacy Access](https://data.ohio.gov/wps/portal/gov/data/view/ohio-pharmacy-assessment-)



## References
[0] Reference




[1] Reference




[2] Reference
