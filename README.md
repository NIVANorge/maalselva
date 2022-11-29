# maalselva

This repository contains data and code from the Målselva river in Troms and Finnmark, Northern Norway. Målselva river is one of NIVA's land-ocean interaction study sites, with a water quality sensor station.

The 2022_MD folder contains data and analyses underpinning a NIVA report on the value of sensor data, with case studies of both Storelva and Målselva. The 2022_FLINK folder contains data and analyses from a small project with NORCE, using the same sensor data as used in 2022_MD, plus combined with remotely sensed snow and wet snow cover data.

Next steps are to carry out analyses for one or two papers:

1) Trends in timing and seasonality of DOC fluxes to the coast (Amanda lead)

2) Målselva DOM fluxes in more detail (hyseteresis, OM sources,...; Leah lead). For this paper, next steps are:

* Make clean notebook just focused on FDOM and Målselva
* FDOM sensor data: 2020 data was removed because of step changes. Try correcting these and add the data back in
* Double-check summer time vs winter time for both sensors and grab samples
* Use raw Q data downloaded from NVE by me
* Add 2020-2022 FDOM data for Målselva. Correct for any step changes
* Look into NIVA DOC data from 2020 onwards. What's going on?! Dodgy across all sites/programmes?
* Look further into FDOM corrections (turbidity, internal shielding effect of high DOM on FDOM). Ask Benoit D for advice.
* Split into different periods: baseflow, snow melt, summer/autumn flow events. See e.g. SimplyP paper and code for ideas
* Look at QC relationships with grab samples as well as sensor data? Double-check that see similar things
* For hysteresis, try out this python package:https://pypi.org/project/hysteresis/ (or this R package looks like it could be useful: https://cran.r-project.org/web/packages/hysteresis/vignettes/index.html)
* Calculate fluxes using logCQ relationships. As good as sensor-based estimates?
* Think more about how to bring the satellite data into the picture
* Download Q data for Barduelva (Øyvind posted the station ID in Teams)
* Look at snow data vs FDOM plots in more detail, as well as interpretation word doc I put together for FLLINK, and think about next steps to make more from this data.
* Look into any diurnal FDOM patterns
