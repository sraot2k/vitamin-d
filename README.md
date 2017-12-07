# vitamin-d

These python jupyter notebooks are part of Root Cause Analysis for my tooth sensitivity and it's fix.

There are two sources of Vitamin D. UVB Rays from Sun and the food.
![Alt text](/images/Vitamin_D_Energy_Source.png?raw=true "Vitamin D Energy Source")

UVB Rays from sun don't reach earth all the time. It depends on the time of the year and place on earth.  The article at https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3897581/ suggests, lesser the zenith angle of the sun higher the Vitamin D production.  The notebook uvb_rays_for_vitamin_d.ipynb computes the best possible time to get into sun for maximum Vitamin D, based on coordinates (Latitude and Longitude) of the location and time of the year. The following is the output of script for Hyderabad city.
![Alt text](/images/SunGraph_Hyderabad.png?raw=true "Sun Graph for Hyderabad")

There are very limited foods with good amount of Vitamin D. The notebook usda_data.ipynb downloads USDA nutritional database from https://www.ars.usda.gov/ARSUserFiles/80400525/Data/SR/SR28/dnload/sr28asc.zip  and converts into a python pandas DataFrame. This DataFrame is used to find the foods with maximum Vitamin D or any other nutrient.

### Installation

Anaconda https://www.anaconda.com/download/ is required along with pysolar and timezonefinder

pip install pysolar

pip install timezonefinder
