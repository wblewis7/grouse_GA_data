# grouse_GA_data
Survery and detection data of ruffed grouse in North Georgia from Lewis et al. "Abundance and distribution of ruffed grouse (Bonasa umbellus) at the southern periphery of the range: Implications for management".

Drumming male grouse were surveyed during the springs of 2020 - 2021 in North Georgia via roadside drumming surveys. Grouse were surveyed at survey points, with survey points grouped together along roadside routes. Observers performed 5-minute 200 m radius point counts, estimating the distance (binned to 20m) to any grouse heard drumming and recording survey-specific covariates. Each sampling point was surveyd ~3 times during each year. This repository contains two dataframes used in analysis.

The first dataframe, RUGR_counts.csv, contains data on the detections of drumming ruffed grouse. "Route" refers to the roadside survey route, while "Point" refers to the survey point along the roadside route. "Date" refers to the date of the survey, "Time" refers to the time (EST) at which the survey was started, and "Distance" refers to the estimated distance band (m) between the observer and the drumming grouse. Note that this dataframe contains only detections and does not contain non-detections. Also note that multiple grouse were detected in the same distance band on some surveys.

The second dataframe, RUGR_drummingsurveys.csv, contains data on drumming surveys of ruffed grouse. "Route", "Point", "Date",and "Time" are the same as in RUGR_counts.csv. "Cloud.Cover" is the percent cloud cover, "Temperature" is the temperature (C), "Wind.Speed" is the wind speed, "Disturbance" is the background noise (number of passing cars), and "Precipitation" ("None","Lt. Rain","Rain") are survey-level covariates. "Wind.Speed" is based on a 5-point Beufort scale. "Disturbance" is based on on a 5-point scale from 1 (no ambient noise) to 5 (intense noise such as constant traffic, completely hampering ability to hear grouse drums). "Replicate" refers to the order of replicate surveys within each year (1 - 6).
