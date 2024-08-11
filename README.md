# broman-etal_2024_erl
**Multi-scale impacts of climate change on hydropower for long-term water-energy planning in the contiguous United States**

Daniel Broman<sup>1\*</sup>, Nathalie Voisin<sup>1,2\*</sup>, Shih-Chieh Kao<sup>3</sup>, Alisha Fernandez<sup>1</sup>, and Ganesh R. Ghimire<sup>3</sup>
and 

<sup>1 </sup> Pacific Northwest National Laboratory, Richland, WA, USA
<sup>2 </sup> University of  Washington, Seattle, WA, USA
<sup>3 </sup> Oak Ridge National Laboratory, Oak Ridge, TN, USA


\* corresponding author: daniel.broman@pnnl.gov and nathalie.voisin@pnnl.gov

## Abstract
Climate change impacts on watersheds can potentially exacerbate water scarcity issues where water serves multiple purposes including hydropower. The long-term management of water and energy resources is still mostly approached in a siloed manner at different basins or watersheds, failing to consider the potential impacts that may concurrently affect many regions at once. There is a need for a large-scale hydropower modeling framework that can examine climate impacts across adjoining river basins and balancing authorities (BAs) and provide a periodic assessment at regional to national scales. Expanding from our prior assessment only for the U.S. federal hydropower plants, we enhance and extend two regional hydropower models to cover over 85% of the total hydropower nameplate capacity and present the first contiguous U.S. (CONUS)-wide assessment of future hydropower production under CMIP6’s high-end SSP5-8.5 emission scenario using an uncertainty-aware multi-model ensemble approach. We present regional hydropower projections, using both BA regions and U.S. Hydrologic Subregions (HUC4s), to consistently inform the energy and water communities for two future periods – the near-term (2020–2039) and the mid-term (2040–2059) relative to a historical baseline period (1980–2019). We find that the median projected changes in annual hydropower generation are typically positive – approximately 5% in the near-term, and 10% in the mid-term. However, since the risk of regional droughts is also projected to increase, future planning cannot overly rely on the ensmble median, as the potential of severe hydropower reductions could be overlooked. The assessment offers an ensemble of future hydropower generation projections, providing regional utilities and power system operators with consistent data to develop drought scenarios, design long duration storage and evaluate energy infrastructure reliability under intensified inter-annual and seasonal variability.

## Journal reference

## Code reference

## Data references

### Origin data
|       Dataset                                       |               Repository Link                |               DOI                |
|:---------------------------------------------------:|:--------------------------------------------:|:--------------------------------:|
|   CMIP6-based Multi-model Hydroclimate Projections  | https://doi.org/10.21951/SWA9505V3/1887469   | 10.21951/SWA9505V3/1887469       |

### Input data

#### wmpy_power static input development
`wmpy_power` requires hydropower facility characteristics including 

|       Dataset       |               Repository Link                |               DOI                |
|:-------------------:|:--------------------------------------------:|:--------------------------------:|
| National Inventory of Dams 'nation file' | https://nid.sec.usace.army.mil/#/downloads   | - |
| National Inventory of Dams API | NONE; see API call) | - |
| Watershed Boundary Dataset (WBD) | https://datagateway.nrcs.usda.gov/catalog/productdescription/wbd.html; https://nrcs.app.box.com/v/huc/folder/39290322977 | - |
| Watershed Boundary Dataset (WBD) | https://datagateway.nrcs.usda.gov/catalog/productdescription/wbd.html; https://nrcs.app.box.com/v/huc/folder/39290322977 | - |
| Existing Hydropower Assets (EHA) Plant Database 9505 Extension v1.0 | https://zenodo.org/records/10520289 | https://doi.org/10.5281/zenodo.10520289 |
| Existing Hydropower Assets (EHA) Plant Database 9505 Point of Diversion v1.0 | https://zenodo.org/records/10520486 | https://doi.org/10.5281/zenodo.10520486 |
| Hydropower Infrastructure - LAkes, Reservoirs, and RIvers (HILLARI) v1.1 | https://hydrosource.ornl.gov/dataset/hydropower-infrastructure-lakes-reservoirs-and-rivers-HILARRI | https://doi.org/10.21951/HILARRI/1781642 |
| Global Reservoir and Dam Database (GRanD) v1.3 | https://www.globaldamwatch.org/directory | https://doi.org/10.1890/100125 |
| Hydropower Energy Storage Capacity Dataset (HESC) v1.0 | https://zenodo.org/records/10520289 | https://doi.org/10.21951/HESC/1822833 |
| mosartwmpy CONUS hydropower facilities v1.0 | https://zenodo.org/records/10520289 | https://doi.org/10.21951/HESC/1822833 |
| CONUS Hydropower Head and Storage | https://zenodo.org/records/10520078 | https://doi.org/10.5281/zenodo.10520078 |

#### runoff data

### Output data
|       Dataset                                                |               Repository Link                |               DOI                |
|:------------------------------------------------------------:|:--------------------------------------------:|:--------------------------------:|
|  CONUS-wide HUC4 Watershed Scale Hydropower Projections      | https://doi.org/10.5281/zenodo.10535564      | 10.5281/zenodo.10535564          |
|  CONUS-wide Balancing Authority Scale Hydropower Projections | https://doi.org/10.5281/zenodo.10535564      | 10.5281/zenodo.10535564          |



## Contributing modeling software
### Pre
|  Model   | Version |         Repository Link                                                 | DOI |
|:--------:|:-------:|:-----------------------------------------------------------------------:|:-:  |
| VIC      | v5.1.0  | https://github.com/UW-Hydro/VIC                                         | -   |
| PRMS     | v5.1.0  | https://www.usgs.gov/software/precipitation-runoff-modeling-system-prms | -   |

### Direct

|  Model   | Version |         Repository Link          | DOI |
|:--------:|:-------:|:--------------------------------:|:---:|
| mosartwmpy | v0.5.0 | https://github.com/IMMM-SFA/mosartwmpy | https://doi.org/10.21105/joss.03221 |
| wmpy_power | v0.2 | https://github.com/9505-PNNL/wmpy_power | - |

## Reproduce my experiment
This experiment relies upon a modeling chain to develop the climate-informed hydropower projections.

![modeling_chain_flowchart](https://github.com/9505-PNNL/broman-etal_2024_erl/tree/main/bin/modeling_chain_flowchart.png?raw=true)




## Reproduce my figures
