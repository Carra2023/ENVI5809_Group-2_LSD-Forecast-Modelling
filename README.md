# ENVI5809 Group 2: Longshore Drift Forecast Modelling
Understanding short term wave climate effects on regional sediment transport using nearshore wave forecast models
![image](https://user-images.githubusercontent.com/90363570/134794322-d775cbea-823a-4597-880e-e816046e7241.png)

# Project Collaborators and contact details

Caitlin May - cmay3858@uni.sydney.edu.au

Carra Williams - carra.williams@sydney.edu.au 

Ian Ahern - iahe9611@uni.sydney.edu.au

Nadine Hargreaves - nhar2545@uni.sydney.edu.au


## Research Objectives:

Build a predictive model that can forecast 7- day longshore sediment transport to highlight regions and magnitudes of accretion and erosional ‘hotspots’ around Tweed Heads and Collaroy, NSW.



## Scientific Questions/Hypothesis

1. Can we use predictive forecast models for longshore sediment transport to identify the locations and magnitudes of erosional ‘hotspots’ along the NSW Coast?
2. Can a predictive model be used to forecast 7- day longshore sediment transport for two highly urbanised regions on the NSW coastline. 
3. What are the magnitudes of LSD from a 7 day forecast? And what impact does this have on the human environment?


## Links to datasets

NSW Nearshore Wave Forecast 
https://forecast.waves.nsw.gov.au/ 

Australian Bathymetric Topographic Grid 2009 
https://data.gov.au/data/dataset/australian-bathymetry-and-topography-grid-june-2009

General NetCDF Files from Manly Hydraulic Labs
http://thredds.aodn.org.au/thredds/catalog/NSW-OEH/Manly_Hydraulics_Laboratory/Wave/Sydney/catalog.html

7 Day forecast and hindcast data from 2011 provided privately by Manly Hydraulics lab via email communication.

Data Table Summary
![image](https://user-images.githubusercontent.com/90363570/134794416-55b121e1-8051-4668-869b-4a2d0e74d263.png)

### Example of data set from wave buoy data offshore Sydney, showing prevailing wave height and direction. Below is a graph plotting the 7 day wave height and direction forecast against real time observations. (Graph and Image Source: Manly Hydraulics Lab Website: https://forecast.waves.nsw.gov.au/index.php?init=1&cont=10&zoom=7&mod=20
![image](https://user-images.githubusercontent.com/90363570/134794932-6ffcdebc-61ae-4192-8792-7474362d6b34.png)






## Summary of Analysis
#Original
This project is designed so that the final model and code will be customizable and we hope to consider it a blueprint model that can be applied to any region around the world with nearshore wave data. 
Wave forecast data (including wave height, direction and period) will be imported to a Jupyter notebook as net CDF files. 
The bathymetric data (Source shown in Figure 1) will be used to extract a contour line at 10m depth as a shapefile and converted to points using a spline funtcion.
The angle of incidence is computed between the contour line and the wave direction, using cKD Tree function to create a search mask and average the data points out for a more representative value. 
Using Airy's linear wave theory calculation, the long shore drift and the divergence of drag are calculated along the contour to identify the regions in accretion and the regions in erosion. 
Finally, these sediment distributions will be represented visually in scatter plots.

## Summary of Analysis
#Revised
This project is designed so that the final model and code will be customizable and we hope to consider it a blueprint model that can be applied to any region around the world with nearshore wave data. 
Wave forecast data (including wave height, direction and period) will be imported to a Jupyter notebook as net CDF files, and the bathymetric data (Source shown in Figure 1) will be used to extract a contour line at 10m depth as a shapefile.
The angle of incidence is computed between the contour line and the wave direction, and then using Airy's linear wave theory calculations, the divergence of drag and then the long shore drift are calculated along the contour to identify the regions in accretion and the regions in erosion. 
Finally, these sediment distributions will be represented visually in scatter plots and through time on an interactive map.

![image](https://user-images.githubusercontent.com/90363570/134795135-59dfae34-283c-43ac-bbd1-81fd15c67e2d.png)

![image](https://user-images.githubusercontent.com/90363570/134794969-b53fc805-801d-472b-a5dd-78beb50b2f10.png)


## Link to Project Repo...





# Project Guidelines
You must have your dataset(s) and general scope for your project approved by the instructor. The approval process works like this:

Create a new public github repo for your project (https://docs.github.com/en/get-started/quickstart/create-a-repo (Links to an external site.))
Add a README.md file which contains the scientific question / hypothesis you plan to investigate, links to the relevant datasets, and a three sentence summary of the analysis you plan to do.
Add a link to your project repo in your Report as supplementary information.
Don’t forget to make your project repo public; otherwise we won’t be able to see it.

For some examples of similar types of students' project you might look at:

Correlation between sea surface temperature and sea ice from 1990 (Links to an external site.) by Shengtao Wang,
An analysis of eddies in the Bay of Bengal (Links to an external site.) by Shannon Bohman 
Analysis of the risks to submarine cables (Links to an external site.) by Amelie Latreille 
Seasonality in Salinity, Temperature, and Currents of the North Atlantic (Links to an external site.) by Joohee Kim 
The affect of geopotential height anomalies on climate extremes (Links to an external site.) by Patric Ryser 
