# EA-water-quality-pollution-analysis

Analysis of Environment Agency datasets in R, examining water quality and environmental pollution incident trends across England.

## Overview

This small project analyses water quality data from the Environment Agency, focusing on key parameters including pH, temperature, and conductivity, alongside a separate analysis of pollution incident records examining the frequency, locations, and pollutant types of incidents.

## Data

Source 1: Environment Agency Water Quality Explorer
- Time period: [2020–2025]
- Selected local authority areas: E06000035 Medway, E07000064 Rother, E06000046 Isle of Wight, E07000091 New Forest
- Variables analysed: pH, Temperature, and Conductivity at 25°C

Source 2: National Data Library/Environmental Pollution Incidents (Category 1 and 2)
- Time period: [2000–2026], as of 10/06/2026

## Methods

- Using R in Positron
- Data cleaning and preprocessing
- Exploratory data analysis (distributions, time series, box plots, map plots)
- Comperative analysis using mean values (column charts)
- Comparative analysis using frequencies (bar charts)

## Key Findings - Water Quality for four selected areas

At the selected local authority area level:
- pH remains within typical natural ranges (5-9), with only minor variability between locations.
- Temperature shows a consistent and strong seasonal pattern at all sites, with similar cyclical behaviour and no clear annual trend.
- Conductivity shows the greatest differences between sites, with all locations exhibiting spikes. Rother and the Isle of Wight show more frequent and larger fluctuations, while Medway and the New Forest are comparatively more stable overall.

Comparative between area levels:
- pH is very similar across locations for each site type, showing only minor variation, indicating consistent underlying water chemistry across regions.
- Temperature is broadly consistent across locations, but sewage and seawater sites show higher average temperatures compared to freshwater and groundwater, reflecting different environmental conditions and influences.
- Conductivity shows the clearest differences, with Medway freshwater standing out as substantially higher than all other locations, while other site types remain relatively low and comparable. This should be investigated.

## Key Findings - Environmental Pollution Incidents across England

- Category 2 (significant) dominates every region and is the most frequent incident type, whereas Category 1 (major) remains the smallest 
- The North-East region has relatively high cumulative counts in categories 2 and 4 compared with other regions
- Category 1 (Major) shows a broad range of pollutant types, indicating that severe incidents are not dominated by a single source but arise from multiple contributors.
- Category 2 (Significant) is clearly dominated by sewage-related pollutants, standing out as the primary driver of this severity level.
- Category 3 (Minor), like Category 4, is largely associated with waste-related materials, suggesting these incidents are generally lower-impact but more routine.
- Category 4 (No impact) is mainly linked to atmospheric pollutants and specific waste materials, reflecting a higher proportion of reported incidents with limited environmental effect.

## Project Structure

- Download_water_data_API.qmd
- Water_quality_analyses.qmd → full analysis in r
- Environmental_pollution_incidents .qmd → full analysis in r
- Water_quality_analyses.html → rendered report
- Environmental_pollution_incidents .html → rendered report
- data/ → raw data files in csv format
- outputs/ → plots and results

## References

Data API retrieval approach adapted from: https://github.com/Westcountry-Rivers-Trust/Get_EA_WaterQuality_R

Environment Agency Water Quality API: https://environment.data.gov.uk/water-quality

Local authority areas: https://www.ons.gov.uk/aboutus/transparencyandgovernance/freedomofinformationfoi/lookuptableforukauthoritycodes2024
