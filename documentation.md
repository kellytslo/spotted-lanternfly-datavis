# Source Data
## Citation
GBIF.org (19 March 2025) GBIF Occurrence Download  https://doi.org/10.15468/dl.cmm22t
## Data Cleaning
I cleaned this data in OpenRefine. This mostly consisted of deleting unwanted columns; I reserved further filtering for the .ipynb file. I then exported the clean data as a new .tsv file.

# Code Referenced
Visualization 1: https://plotly.com/python/scatter-plots-on-maps/
Visualization 2: https://plotly.com/python/filled-area-plots/

# Methodology
## Data Preparation
I wanted to engineer a sorting feature that would let the viewer filter observations by state, so I had to group the observations by year and location.
## Plot Selection
There were two main patterns I wanted to illustrate: (1) change in range over time and (2) change in population over time. For the first pattern, I needed to convey geospatial information, so I chose an animated bubble map. I used a filled area plot for my second visualization because it allows for easy visual comparison across states.

# Critical Analysis
## Limitations
Because iNaturalist observations are crowdsourced, my data lends itself to spurious correlation — areas with more observations might indicate more observers instead of more spotted lanternflies. Additionally, the bubbles' sizes and colors both indicate the density of observations in a given area, so they're arguably redundant. 
## Potential Improvements
I'd like to implement more visual clarity in the map visualization by changing the opacity of the bubbles and layering them by size. I'm also planning on converting this project to a dashboard app for easier viewing. Beyond that, I'd be interested in doing some kind of centrality analysis on this data — perhaps I could gain insight into whether the SLF invasion has been sustained primarily through local reproduction or repeated foreign imports.
