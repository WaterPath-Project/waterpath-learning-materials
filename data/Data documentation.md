## Conceptual framework

The WaterPath Toolkit uses a conceptual framework that identifies and categorizes the drivers of pathogen pollution and the resulting environmental state.

Scenario inputs are categorized as **Drivers**: the social, agricultural, and infrastructure factors that quantify sources of contamination. Under specific hydrological conditions, these drivers exert **Pressures** on the environment through annual pathogen loads. This results in an environmental **State** characterized by pathogen concentrations in surface water.

The framework also measures **Impact** by translating pathogen concentrations into risk. By incorporating exposure pathways such as drinking water and recreational use, the Toolkit models human intake and calculates the resulting probability of infection.

<div class="framework rounded-lg shadow-sm bg-white border hover:border-sand-100">
<h3 class="flex items-center gap-3"><img src="./figures/human_emissions.svg" width="64" height="64" alt=""/>Human emissions</h2>

<h4 class="flex items-center gap-3"><img src="./figures/human_population.svg" width="48" height="48" alt=""/>Population</h3>

Defines the population in each reporting area and the share living in urban settings. It includes the proportion of children under five and the Human Development Index. These values determine the scale and spatial distribution of human emissions.
<hr/>
<h4 class="flex items-center gap-3"><img src="./figures/sanitation.svg" width="48" height="48" alt=""/>Sanitation</h3>

Defines the mix of toilet facilities used by urban and rural populations. Services are summarized as safely managed, basic, unimproved, and open defecation. The facility mix controls how much human excreta is contained, treated, or released to soil and water.
<hr/>
<h4 class="flex items-center gap-3"><img src="./figures/wastewater_treatment.svg" width="48" height="48" alt=""/>Wastewater treatment</h3>

Defines treated sewage and fecal sludge fractions by area, or individual treatment plant locations and capacities. It supports primary, secondary, tertiary, and quaternary treatment levels. Treatment choices determine the fraction of pathogens remaining in effluent before discharge.
</div>

<div class="framework rounded-lg shadow-sm bg-white border hover:border-sand-100">
<h3 class="flex items-center gap-3"><img src="./figures/livestock_emissions.svg" width="64" height="64" alt=""/>Livestock emissions</h2>

<h4 class="flex items-center gap-3"><img src="./figures/livestock_population.svg" width="48" height="48" alt=""/>Livestock population</h3>
Defines animal numbers by species and geographic area. It includes biological parameters such as prevalence, excretion, body mass, and manure production. Together, these inputs determine the amount of manure-generated pathogen load from livestock.
<hr/>
<h4 class="flex items-center gap-3"><img src="./figures/manure_management.svg" width="48" height="48" alt=""/>Manure management</h3>
Defines the share of each animal group's manure assigned to storage, spreading, grazing, digestion, burning, and other systems. It also divides manure between grazing and other land pathways for intensive and extensive production. These management choices affect pathogen survival and the route by which manure reaches land and surface water.
<hr/>

<h4 class="flex items-center gap-3"><img src="./figures/production_systems.svg" width="48" height="48" alt=""/>Production systems</h3>

Defines the share of each animal group raised in intensive and extensive systems. The production split changes where manure is concentrated and how livestock emissions enter the environment.
</div>

<div class="framework rounded-lg shadow-sm bg-white border hover:border-sand-100">
<h3 class="flex items-center gap-3"><img src="./figures/concentrations.svg" width="64" height="64" alt=""/>Concentrations</h2>
<h4 class="flex items-center gap-3">Hydrology</h3>
Describes river discharge, surface runoff, river temperature, and solar radiation across the scenario. Discharge and runoff control dilution, downstream transport, and the movement of pathogens from land into rivers. Water temperature and solar radiation influence pathogen die-off and therefore the concentrations that remain in surface water.
</div>

<div class="framework rounded-lg shadow-sm bg-white border hover:border-sand-100">
<h3 class="flex items-center gap-3"><img src="./figures/risk.svg" width="64" height="64" alt=""/>Risk</h2>
<h4 class="flex items-center gap-3">Exposure pathways</h3>
Defines exposure pathways including drinking water, swimming, flooding, open drains, children's play, and clothes washing. It controls exposure frequency, ingested volume, drinking-water treatment, and boiling assumptions. These settings drive the quantitative microbial risk assessment calculation that converts pathogen concentrations into infection risk.
</div>

## Structured data management

The WaterPath Toolkit streamlines the processing of data required for waterborne pathogen modelling according to this framework. Its tools and learning materials support both the acquisition of data from heterogeneous sources and their consolidation into a common format for modelling.

The Toolkit uses well-known, flexible standards such as [Table Schema](https://specs.frictionlessdata.io/table-schema/) and formats such as CSV and JSON. This keeps the workflow accessible and enables researchers to create and share reproducible data resources tailored to their own modelling use cases.

### Data categories and sources

The data ecosystem follows the framework's four categories: Human emissions, Livestock emissions, Concentrations, and Risk. These categories align with the requirements of the [GloWPa model](https://git.wur.nl/glowpa/glowpa-r), an integral component of the Toolkit.

The categories draw primarily on multiple data sources, including scientific databases, open datasets, and peer-reviewed publications. Each source is processed individually to harmonize how data is retrieved and linked across the Toolkit. Priority is given to sources most likely to be adapted or modified by GloWPa users. Foundational inputs, such as pathogen properties and gridded population datasets, are excluded from this workflow because they represent core scientific assumptions of the model.

Α full list of data sources is available in the [online documentation](https://waterpath-toolkit.org/docs/data-sources/). These sources can be consolidated into a single input file using the Toolkit's input [Data Preparation Tool](https://waterpath-toolkit.org/model/). Each dataset includes its original raw data, accompanying metadata, and Python scripts that allow users to generate new, reusable records in the same standardized format.

### Data explanation and schemas

All variables used by the WaterPath Toolkit are documented using the [Table Schema specification](https://specs.frictionlessdata.io/table-schema/). Interactive documentation is available on the [Data Explanation page](https://waterpath-toolkit.org/docs/data-explanation/).
