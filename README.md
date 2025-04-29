# SP2025-FP07-glaciermelt
Final project repo for the glacier melt runoff effect on ocean current 

## Group Members:
- Raquel Dickinson
- Aucklynn Sacco
- Anna George

## Project Summary: 
With global temperatures rising, one of Earth's two ice sheets, Greenland, have been melting more rapidly, introducing large amounts of freshwater into the Arctic and North Atlantic ocean. This introduction of freshwater alters ocean salinity, which may weaken ocean currents.

## Using this Repository
/data/: contains smaller data sets made from larger data sets

/notebooks/: main Jupyter notebooks for each analysis step:

current_analysis.ipynb: cleaning and analysing current

greenland-mass-plot.ipynb: cleans and plots greenland mass

relating-previous-plots.ipynb: relates all of the cleaned data and tests correlation

salinity_analysis_dev.ipynb: cleans and plots salinity data

surface-velocioty-lot.ipynb: cleans and plots surface velocity data

README.md: project overview, instructions, and findings

**To Use this Repository:** 

1. Clone the repository
2. Download the data
   a. [Greenland Mass Loss](https://www.epa.gov/climate-indicators/climate-change-indicators-ice-sheets)
   b. [Salinity] (https://sio-argo.ucsd.edu/RG_Climatology.html)
   c. [Ocean Currents] (https://doi.org/10.48670/mds-00327.)
3. Run notebooks in order using Jupyter Lab 


## Introduction 
Accelerated glacial melt has been a concern for many reasons in recent times, one of which is the potential that this melt will weaken ocean currents. An analysis done on the Atlantic ocean currents specifically predicts that the weakening of these currents will lead to a significant decrease in temperatures in North American and parts of Eurasia [1]. This is because the Gulf Stream, the major ocean current in the north Atlantic, circulates warmer waters from the equator up towards Greenland, where the water cools and sinks, traveling back down the the equator. If the Gulf Stream ceases to perform this circulation, the warm water near the equator will not travel northward [1]. Greenland is generally melting at a faster rate than Antarctica, hence the general focus on the northern oceans, but both ice sheets average out to have hundreds of billions of tons of melting each year [2]. With Greenland and Antarctica holding about 99% of the Earth's freshwater ice, this mass introduction of freshwater, which appears to increase each year, could drastically change the ocean's salinity, thus disrupting the ocean currents [1][2].

### Problem Statement:
We are going to analyze how the Greenland ice sheet melting impacts ocean salinity and see if that has an affect on deep-sea currents.

### Questions:
- What are the potential effects of declining salinity on deep-sea currents?
- How has glacier mass loss from Greenland contributed to changes in ocean salinity over time?
- How do variations in ocean salinity correspond to shifts in ocean surface currents and deep-water circulation patterns?

### Objectives:

- Analyze changes in glacier melt over time
- Analyze changes in salinity over time
- Analyze changes in ocean current over time
- Piece together data to see if there is an association between glacier melt and changes in ocean current using change in salinity.

## Tools/Packages
We will use the following tools and packages for data analysis, visualization, and statistical computations:
- [Pandas](https://pandas.pydata.org/) – For loading, cleaning, and manipulating large datasets.  
- [Matplotlib](https://matplotlib.org/) – For creating plots and visualizing trends over time.  
- [NumPy](https://numpy.org/) – For numerical computations, especially handling arrays and large datasets.  
- [SciPy](https://scipy.org/) – For performing statistical analysis, such as correlation tests.
- [XArray](https://xarray.dev/) - For simplifying multi-dimensioned arrays
- [HvPlot](https://hvplot.holoviz.org/) - For visualizing data
- [GeoViews](https://geoviews.org/) - For visualizing geographic data 
- [netCDF4](https://unidata.github.io/netcdf4-python/) – For working with netCDF files, a common format for climate and oceanographic data.
- [Jupyter Notebook](https://jupyter.org/) – For interactive analysis, combining code, explanations, and visualizations in one document.  
- [NASA Earthdata Tools](https://earthdata.nasa.gov/) – For accessing, downloading, and visualizing NASA climate datasets.

## Project Methodology/Approach 
- Data Collection and Preprocessing
  -  Download Necessary Data Sets as listed in Data Sets section.
  -  Clean and organize Data in seperate notebooks
    - This would include identifying any missing data, converting all data into comparable formats, combining data sets that can be combined, removing blatant anomolies, etc.
- Analysis of Glacier Melt Over Time
   - Plot the mass changes of Greenland ice sheet over time.
   - Identify trends of mass loss, which shows rate of ice loss.
- Analysis of Ocean Salinity Over Time
    - Examine time-series data on salinity, focusing on regions affected by glacial melt like the North Atlantic ocean.
    - Visualize changes with hope to show major salinity loss near melting glaciers.
 - Analysis of Ocean Currents Over Time
     - Analyze OSCAR surface current data and look for variations over time that might be linked to decreasing salinity as shown by changes in time.
     - Specifically we will focus where there is more likely to be a change from silinity, again the atlantic ocean.
 - Correlation Analysis
     - Perform statistical analysis to examine basic correlations between glacier melt, salinity changes, and ocean current shifts.
     - If there is changed in ocean current that correlate to changes in salinity that can be easily compared using visuals.
  - Visualizations and Conclusions
      - Though we might have been creating visualizations along the way, if we have not then we will be sure to create them now.
      - Use these visualizations to prove our conlcusions, and reate clear plots and maps that visualize trends and relationships.
     
## Results Summary 

After analysing the data on ocean salinity over time from Argo floats climatology data around Greenland. We see a decrease in salinity over time, averaging a decrease in 0.05388 PSU/decade [3]. Doing a correlation test we get a moderate negative correlation between mass loss and salinity. This shows that as Greenland loses ice more rapidly, salinity tends to drop. This shows what we would expect to see because as freshwater melts into the ocean we get more dilution. From this test, we also see mass loss and current have a weak positive correlation, showing that there is a slight tendency that ice loss increases ocean strengths. We also get that salinity and current have a weak negative correlation so there is a slight tendency for high salinity to cause slower currents. 

The overall trend showed a general increase in ocean current strength, which goes against the hypothesis. One reason this may have been our result is because the sea ice breaking off of Greenland could be churning the surface of the water, thus increasing sea surface velocity. Deep ocean currents may have experienced a different effect, and this is something that future research should explore.

## Challenges 
- Some of the challenges we faced were finding datasets in formats we were able to use. There was a lot of data that was difficult to access due to size/needing another platform to download the data. We also had a hard time finding data that matched years. 
- 
## Contribution Statement

**Aucklynn**: Did salinity analysis. Did correlation analysis. Finished README.md File. 

**Raquel**: I found data for Greenland mass balance and loss over time, and I found the data for ocean current analysis.  I analyzed Greenland mass loss data and ocean current data. I edited the presentation and completed cited all sources and datasets in IEEE. 

**Anna**: Took data from previous graphs and combined to relate in one graph. Created and updated evironemt.yml. Made presentation. 

## References 
- [1] R. van W. US Henk A. Dijkstra, Michael Kliphuis, The Conversation, “If the Atlantic Ocean Loses Circulation, What Happens Next?,” Scientific American. https://www.scientificamerican.com/article/if-the-atlantic-ocean-loses-circulation-what-happens-next/
- [2]“‘Devastating’ melt of Greenland and Antarctic ice sheets is found,” NBC News. https://www.nbcnews.com/science/environment/devastating-melt-greenland-antarctic-ice-sheets-found-rcna80616

## Datasets: 
- [1] US EPA, “Climate Change Indicators: Ice Sheets,” www.epa.gov, Mar. 18, 2021. https://www.epa.gov/climate-indicators/climate-change-indicators-ice-sheets
- [2] “Roemmich-Gilson Argo Climatology,” Ucsd.edu, 2019. https://sio-argo.ucsd.edu/RG_Climatology.html (accessed Apr. 24, 2025).
- [3] “Global Total (COPERNICUS-GLOBCURRENT), Ekman and Geostrophic currents at the Surface and 15m,” Copernicus.eu, 2025, doi: https://doi.org/10.48670/mds-00327.

