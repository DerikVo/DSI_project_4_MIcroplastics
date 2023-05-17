# DSI_project_4
Microplastic project


Project Members

Derik Vo

Veda Patel

Yasser Siddiqui


## Working Problem statement

According to Meijer et al., (2021) over 80% of the global annual emissions of plastic in the ocean come from 1000 rivers. Plastic waste has gone from 1.5 million tons in 1950 to 365 million tons in 2020, and is expected to double by 2025 (Alberghini et al., 2023). Alberghini and team suggest that humans ingest a significant amount of microplastics through food, especially fish and other seafood. The effects of these chemicals range from mutating DNA, reproductive harm, cause cancer,  disrupt hormones, and cause harm to organs (Campanale et al., 2020).

The goal of this project is to identify which regions have the highest concentration of microplastics and building a time series model to try to predict plastic concentrations over time, as well as provide target dates with expected plastic concentrations(eg 2025-2030). With this knowledge we can focus clean up efforts within those regions to help reduce these future numbers. 

## Data Dictionary

Our data is sourced from ['The national Centers for Environmental Information')](https://experience.arcgis.com/experience/b296879cc1984fda833a8acc93e31476) 

|Column|Description|Missing Values|
|-----|-----|----|
|FID|The identifier for the record|0|
|Date|Specific date record was collected format is month/day/year|0|
|Latitude|The north or south angular distance from of the earths equator |0|
|Longitude|The west or west angular distance from of the earths meridian|0|
|Oceans|The specific ocean the record was collected from|0|
|Regions|The specific region (major sea) within an ocean|10052|
|Sub Regions|The specific subregion of a major sea or ocean|12932|
|Microplastics Measurement|micro plastic concentration measured in m^3|0|
|Unit|||
|Density Class Range||0|
|Density Class||0|
|Sampling Method|The specific method used to [collect samples](# sampling method) (will need to create a header for sampling methods)|0|
|Short Reference|Short reference ID|0|
|Long Reference|Long reference ID|0|
|DOI|Digital object identifier||
|Organization|Specific organization that collected the sample|0|
|Keywords|Description of the data|87|
|NCEI Accession Number||0|
|NCEI Accession Link||0|

## Hypothesis

## EDA

During our Exploratory data analysis project we found that Sub Regions and Regions had the highest number of missing values. Upon further inspection we identified this was due to not being entered by the initial researchers. So we used an API to use the longitudinal and latitudinal to find the regions and sub regions using Geopy.

When looking at measurements we found a huge range of values. When looking at the quartile ranges we identified the 75% was under 1, but had a max value of over 60,000. We originally thought these outliers were due to a mistake, but when we group them by sampling method we noticed the ranges differed depending on the sampling method. However, there are still some outliers that will need to be investigated.


## Modeling

## Results

## Conclusions
