# 20cr_lawdome

This repository contains code and data for Nilssen et al. (submitted May 2024), "Evaluating the Twentieth Century Reanalysis Version 3 with synoptic typing and East Antarctic ice core accumulation", submitted to Climate of the Past

DATA FILES:

SOM_20CR_4_3_1000.nc - 
NetCDF file of the composite maps of the 12 SOM nodes

SOM_20CR_4_3_1900.csv - 
CSV file of each date from 1 Jan 1900 to 31 Dec 2015, where each date is assigned one of the 12 SOM nodes

som_temporal_correlations_r.csv - 
CSV file with each date from 1 Jan 1900 to 31 Dec 2015, the node for each date, and the pearson pattern correlation score for each date

dss_winter.csv - 
CSV file of annual snowfall accumuluation (metres ice equivalent) at Dome Summit South, Law Dome, 1836-2015. Available from https://data.aad.gov.au/metadata/records/fulldisplay/DSS_2k_data_compilation

assim_obcount_study_area.nc - 
NetCDF file of the number of assimilated observations in ISPDv4.7, on a 2x2 degree grid. Downloaded from https://psl.noaa.gov/data/20CRv3_ISPD_obscounts/, then subset to the study area (30-75S, 40-180E)

sprate_1900_2015_small.nc - 
NetCDF file of 20CRv3 daily mean 3-hourly precipitation rate (65-69S, 110-115E). Downloaded from NCI, also available at https://psl.noaa.gov/data/gridded/data.20thC_ReanV3.html

daily_node_precip.csv - 
CSV file with each date from 1 Jan 1900 to 31 Dec 2015, along with the following for each day: node, 20CRv3 daily precip (mm) at LD coordinates (67S, 113E), precipitation type (zero, normal (<90th percentile), high (90-99th percentile), extreme (>99th percentile))

annual_accum_precip_LD.csv - 
CSV file with each year from 1900 to 2015, with the annual snowfall accumulation at DSS (m ice equivalent), and the annual precip amount (mm) at LD coordinates (67S, 113E)

CODE FILES:

SOM code: - 
soms1900_4_3.Rmd (this requires a NetCDF file of 500hPa geoptential height daily anomalies over the study region, which is a large file - around 1.1GB. This data is available from https://psl.noaa.gov/data/gridded/data.20thC_ReanV3.html, but will require joining multiple files together (one per year) and then subsetting for the study area)

Code for generating datasets: - 
making_datasets.Rmd (this makes daily_node_precip.csv and annual_accum_precip_LD.csv)


Code for making figures: 
fig02_precip_accum.Rmd, 
fig04_obs_types_nodes.Rmd, 
fig05_boxplot_barplot.Rmd, 
linear_models_fig06.Rmd, 
somcor_histograms.Rmd 

Code for tables: 
table1.Rmd, 
table3_corrs.Rmd, 
trend_table.Rmd, 

Code for statistical tests regarding the 20CR daily precipitation associated with each node:
node_precip_tests.Rmd
