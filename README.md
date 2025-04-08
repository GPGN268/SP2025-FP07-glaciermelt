# SP2025-FP07-glaciermelt
Final project repo for the glacier melt runoff effect on ocean current 

## Group Members:
- Raquel Dickinson
- Aucklynn Sacco
- Anna George

## Summary:
With global temperatures rising, Earth's two ice sheets, Greenland and Antarctica, have been melting, introducing large amounts of freshwater into the ocean. This introduction of freshwater alters ocean salinity, which may weaken ocean currents.

## Introductory Background Information:
Accelerated glacial melt has been a concern for many reasons in recent times, one of which is the potential that this melt will weaken ocean currents. An analysis done on the Atlantic ocean currents specifically predicts that the weakening of these currents will lead to a significant decrease in temperatures in North American and parts of Eurasia [1]. This is because the Gulf Stream, the major ocean current in the north Atlantic, circulates warmer waters from the equator up towards Greenland, where the water cools and sinks, traveling back down the the equator. If the Gulf Stream ceases to perform this circulation, the warm water near the equator will not travel northward [1]. Greenland is generally melting at a faster rate than Antarctica, hence the general focus on the northern oceans, but both ice sheets average out to have hundreds of billions of tons of melting each year [2]. With Greenland and Antarctica holding about 99% of the Earth's freshwater ice, this mass introduction of freshwater, which appears to increase each year, could drastically change the ocean's salinity, thus disrupting the ocean currents [1][2].

## Problem Statement, Questions and Objectives: 

**Problem Statement:** We are going to analyse how glacier melt impacts ocean salinity and see if that has an affect on deep-sea currents. 

**Questions:**  
- What are the potential effects of declining salinity on deep-sea currents?
- How has glacier mass loss from Greenland, Antarctica, and Alaska contributed to changes in ocean salinity over time?
- How do variations in ocean salinity correspond to shifts in ocean surface currents and deep-water circulation patterns?
- Are there regional differences? 

**Objectives:**
- Analyze changes in glacier melt over time 
- Analyze changes in salinity over time
- Analyze changes in ocean current over time
- Piece together data to see if there is an association between glacier melt and changes in ocean current using change in salinity. 

## Data Sets: 
**We are unsure about these datasets, we are having a really hardtime finding usable data - these did not have data we were able to download but kept them because they are the only ones we have** 
- See data folder for downloaded data, and see notebooks folder for data analysis

- [ESA Sea furcace Salinity](https://catalogue.ceda.ac.uk/uuid/ecc355e395ed4c5597c613ae7f9c53b0/)
- [OSCAR Surface Currents](https://podaac.jpl.nasa.gov/dataset/OSCAR_L4_OC_INTERIM_V2.0)
- [NASA Earthdata - Greenland Icesheet](https://cmr.earthdata.nasa.gov/search/concepts/C2548143452-FEDEO.html)
- [Datasheet - Greenland and Antarctic Ice Sheet Melt](https://www.nasa.gov/wp-content/uploads/2023/06/antarcticicemass-classroomdatasheet.pdf?emrc=636650)
- [USGS Alaska Science Center - Glacier Wide Mass Balance](https://alaska.usgs.gov/products/data.php?dataid=79)
- [NSIDC - Global Glaciers](https://nsidc.org/data/glims)

## Tools and Packages:
We will use the following tools and packages for data analysis, visualization, and statistical computations:
- [Pandas](https://pandas.pydata.org/)** – For loading, cleaning, and manipulating large datasets.  
- [Matplotlib](https://matplotlib.org/)** – For creating plots and visualizing trends over time.  
- [NumPy](https://numpy.org/)** – For numerical computations, especially handling arrays and large datasets.  
- [SciPy](https://scipy.org/)** – For performing statistical analysis, such as correlation tests.  
- [netCDF4](https://unidata.github.io/netcdf4-python/)** – For working with netCDF files, a common format for climate and oceanographic data.
- [Jupyter Notebook](https://jupyter.org/)** – For interactive analysis, combining code, explanations, and visualizations in one document.  
- [NASA Earthdata Tools](https://earthdata.nasa.gov/)** – For accessing, downloading, and visualizing NASA climate datasets.  

## Planned Methodology:
- Data Collection and Preprocessing
  -  Download Necessary Data Sets as listed in Data Sets section.
  -  Clean and organize Data.
  -  This would include identifying any missing data, converting all data into comparable formats, combining data sets that can be combined, removing blatant anomolies, etc.
- Analysis of Glacier Melt Over Time
   - Plot the mass changes of Greenland, Antarctica, and Alaskan glaciers over time.
   - Identify trends of mass loss, which shows rate of ice loss.
- Analysis of Ocean Salinity Over Time
    - Examine time-series data on salinity, focusing on regions affected by glacial melt like the atlantic ocean.
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
     
## Expected Outcomes:
We expect to see from our data sets that the mass lost in Greenland and Antarctica is significant and has been increasing over the years, that the overall salinity of the oceans, particularly the Atlantic and Arctic oceans, has gone down over the years, and that the ocean currents have been weakening over the years.

## Challanges: 
Currently, the biggest challenge is finding usable and relavant data. Most data on the topic are separated in different data sets by year, making it a challenge to comprehensively analyzie trends over time. We are looking into finding a better process to find viable data sets.

## References
- [1] R. van W. US Henk A. Dijkstra, Michael Kliphuis, The Conversation, “If the Atlantic Ocean Loses Circulation, What Happens Next?,” Scientific American. https://www.scientificamerican.com/article/if-the-atlantic-ocean-loses-circulation-what-happens-next/
- [2]“‘Devastating’ melt of Greenland and Antarctic ice sheets is found,” NBC News. https://www.nbcnews.com/science/environment/devastating-melt-greenland-antarctic-ice-sheets-found-rcna80616
‌
