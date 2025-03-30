# Forest_fires_timeseries
Monitoring fires in Brazil in 2024

## Importing region shapefile and satellite images
First I tried to use the shapefile of Brazil was obtained from geoboundaries (1) and can be found in the folder region. However, this resulted in exceeded memory usage in GEE.
Instead, the geometry shapefile was roughly handdrawn directly in GEE.
For the analysis, Sentinel-2 images were used due to:
- high spatial resolution
- sufficient temporal resolution

To-do: Use MODIS to also monitor the long-term fire activity in Brazil since 2000 and correlate them with climate variations

## Filtering images 
Only images from summer 2024 were used - between 1st of June and 1st of September
The images were filtered for the area of Brazil and only those with less then 20% cloud cover were kept



## Sources
1) Runfola, D. et al. (2020) geoBoundaries: A global database of political administrative boundaries. PLoS ONE 15(4): e0231866. https://doi.org/10.1371/journal.pone.0231866
