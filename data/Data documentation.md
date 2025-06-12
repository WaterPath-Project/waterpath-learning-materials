# About WaterPath Toolkit Data

## Introduction

Our open-source toolkit is designed to streamline the processing of data that can be used for waterborne pathogen modelling. It offers a set of tools and learning material, that enable: a) data acquisition from heterogenous data sources and b) their consolidation into a common format that can be used for modelling purposes. To that end, we have adopted a set of well-known and flexible standards (such as [Tableschema](https://specs.frictionlessdata.io/table-schema/)) and formats (such as CSV and JSON), aiming to keep the workflow as simple and accessible as possible for a broad audience. We hope this approach empowers researchers to create and share reproducible data resources tailored to their own modelling use cases.

## Data categories 

The WaterPath Toolkit has organized its data ecosystem in four key categories, aligned with the requirements of the [GloWPa model](https://git.wur.nl/glowpa/glowpa-r), which is an integral component of the Toolkit. These categories are: 

<div class="mt-12 mb-12 w-full grid md:grid-cols-4 gap-4 mx-auto m-auto items-stretch"><div class="m-auto h-[120px] text-center pt-8 text-lg line-clamp-2 align-middle max-w-sm p-6 rounded-lg shadow-sm bg-white w-full"><h5 class="mb-6 font-bold tracking-tight text-blue-500">Human Emissions</h5></div><div class="m-auto h-[120px] text-center pt-8 text-lg line-clamp-2 align-middle max-w-sm p-6 rounded-lg shadow-sm bg-white w-full"><h5 class="mb-6 font-bold tracking-tight text-blue-500">Livestock Emissions</h5></div><div class="m-auto h-[120px] text-center pt-8 text-lg line-clamp-2 align-middle max-w-sm p-6 rounded-lg shadow-sm bg-white w-full"><h5 class="mb-6 font-bold tracking-tight text-blue-500">Concentrations</h5></div><div class="m-auto h-[120px] text-center pt-8 text-lg line-clamp-2 align-middle max-w-sm p-6 rounded-lg shadow-sm bg-white w-full"><h5 class="mb-6 font-bold tracking-tight text-blue-500">Risk</h5></div></div>

Our data categories primarily pull data from a total of **24 data sources**, which include scientific databases, open datasets and peer-reviewed publications. We are currently processing each source individually to harmonize how data is retrieved and linked across the Toolkit. Priority is given to sources that are most likely to be adapted or modified by users of the GloWPa model, while foundational inputs—such as pathogen properties or gridded population datasets—are excluded from this workflow, as they represent core scientific assumptions of the model.

For the **Human Emissions** category, we have already published the full list of data sources in our [online documentation](https://waterpath-toolkit.org/docs/data-sources/). TThese sources can be consolidated into a single input file using the [Input Data Preparation Tool](https://waterpath-toolkit.org/model/), included in the Toolkit. Each dataset is provided with its original raw data, accompanying metadata, and Python scripts that allow users to generate new, reusable records in the same standardized format.

## Data explanation and schemas

All data variables that are used by the WaterPath Toolkit are documented using the [Tableschema specification](https://specs.frictionlessdata.io/table-schema/). An interactive documentation can be found in our [Data Explanation page](https://waterpath-toolkit.org/docs/data-explanation/).
