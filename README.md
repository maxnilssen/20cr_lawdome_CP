# 20cr_lawdome

This repository contains code and data for Nilssen et al. (submitted May 2024), "Evaluating the Twentieth Century Reanalysis Version 3 with synoptic typing and East Antarctic ice core accumulation", submitted to Climate of the Past

DATA FILES:

SOM_20CR_4_3_1000.nc
NetCDF file of the composite maps of the 12 SOM nodes

SOM_20CR_4_3_1900.csv
CSV file of each date from 1 Jan 1900 to 31 Dec 2015, where each date is assigned one of the 12 SOM nodes

dss_winter.csv
CSV file of annual snowfall accumuluation (metres ice equivalent) at Dome Summit South, Law Dome, 1836-2015. Available from https://data.aad.gov.au/metadata/records/fulldisplay/DSS_2k_data_compilation

assim_obcount_study_area.nc
NetCDF file of the number of assimilated observations in ISPDv4.7, on a 2x2 degree grid. Downloaded from https://psl.noaa.gov/data/20CRv3_ISPD_obscounts/, then subset to the study area (30-75S, 40-180E)

sprate_1900_2015_small.nc
NetCDF file of 20CRv3 daily mean 3-hourly precipitation rate (65-69S, 110-115E). Downloaded from NCI, also available at https://psl.noaa.gov/data/gridded/data.20thC_ReanV3.html



CODE FILES:

Code for making figures:
fig02_precip_accum.Rmd

fig04_obs_types_nodes.Rmd

fig05_boxplot_barplot.Rmd

fig05_boxplot_barplot.Rmd

