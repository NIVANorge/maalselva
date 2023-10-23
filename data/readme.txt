# River inputs for Målselva

Leah Jackson-Blake (leah.jackson-blake@niva.no), 2023-10-23

Files in folder:

## Q_målselva_daily-mean_area-scaled_2017-2022.csv

Daily mean discharge in m3/second, estimated for the NIVA monitoring site (catchment area 5586 km2). Based on area-scaling data from the NVE gauging site 15 km upstream (Målselvfossen, station ID 196.35.0; catchment-area 3039 km2). N.B. this area-scaling is an approximation, and assumes the same discharge and dynamics in the other (unmonitored) half of the catchment. In reality, the unmonitored part includes Barduelva which has a large lake in its headwaters and is regulated, so we would expect a more lagged/smooth rainfall-runoff signal than at Målselvfossen. This will be investigated further in the future. 

The whole Målselvvassdraget/Malangen vassdragsområde has an area of 6676 km2 (including all the smaller rivers out to Malangen; see NVE Atlas for the boundary). If interested in runoff from the whole land area to the larger fjord area, you might want to area-scale this discharge (i.e. multiply it by 6676 / 5586).


## malselva_sensor_daily_2018-2021.csv

Daily mean values derived from the NIVA sensor station on Målselva. Includes river water temperature, which may be useful for marine modelling. Can be easily updated to include 2022.

Parameters:
- T_water (degC)
- FDOM (fluorescing dissolved organic matter; ug/L)
- Conductivity (mS/m)
- pH
- Turbidity (NTU)

## malselva_waterchem_raw-grab-samples_2018-2022.csv

Water chemistry data from elveovervåkingsprogrammet. Same location as the NIVA sensors. I just picked out variables that may be of interest, and did a little cleaning/merging of variables. Hopefully the variable names are self-explanatory, except perhaps some of the N and P species:
- N_Part: particulate N
- TOTN: total N
- TRP: total reactive P (i.e. dissolved + particulate reactive P)
- TP: total P
- TDP: total dissolved P
- PP: particulate P
- SPM: suspended particulate matter

Si and SiO2 were analysed separately using different methods.

N.B. pre-2018 water chemistry data is a available, but from a different site 15 km upstream of the current site, upstream of a major tributary (Barduelva). Can be extracted if desired though.

All units are provided in sheet "water_chem_units.csv"


## malselva_waterchem_daily_interpolated_2018-2022.csv"

Simple linear interpolation of the raw grab samples to generate a daily time series. Alternative and potentially better methods are available, some of which we have looked into (e.g. using FDOM sensor data to estimate daily DOC concentrations). If this is of interest, we can spend a day updating this.

