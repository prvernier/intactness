# Intactness Project

Revised: 2022-11-17


Comparison of intactness datasets for conservation planning in the boreal region of North America.


## Manuscript

Vernier, P.R., Leroux, S.J., Cumming, S.G., Lisgo K., Suarez Esteban A., Krawchuck, M.A., Schmiegelow, F. 2022. Comparing global and regional maps of intactness in the boreal region of North America: implications for conservation planning in one of the world's remaining wilderness areas. URL: https://www.frontiersin.org/articles/10.3389/ffgc.2022.843053/full


## Supplementary material

* [Description of intactness and human influence datasets within the boreal region of Canada and Alaska.](https://github.com/beacons/intactness/blob/master/supp/s1_datasets.md)
* [Interactive maps for the two case studies.](https://rpubs.com/vernier/intactness_case_studies)


## Code

The following scripts can be used to replicate the analysis. Links to download the required datasets can be found in the [s1_datasets.md](https://github.com/beacons/intactness/blob/master/s1_datasets.md). Check the top of each script to determine which datasets are needed. If you have any questions, please contact: pierre.vernier@gmail.com

### Prepare data

  - 01_gen_canada_data.R - Prepare datasets for coverage estimation within Brandt's boreal region in Canada
  - 02_gen_alaska_data.R - Prepare datasets for coverage estimation within Brandt's boreal region in Alaska

### Calculate intact area estimated by each dataset

  - 03_calc_canada_area.R - Calculate the area of each dataset within the Canadian boreal region
  - 04_calc_alaska_area.R - Calculate the area of each dataset within the Alaska boreal region
  - 05_gen_canada_maps.R - Create png maps of the distribution of each dataset within the Canadian boreal region
  - 06_gen_alaska_maps.R - Create png maps of the distribution of each dataset within the Canadian boreal region

### Estimate agreement among datasets

  - 07_prep_agree_data.R - Create 1-km intactness rasters for area of intersection among all datasets
  - 08_calc_agreement.R - Calculate Jaccard index among intactness rasters

### Validation of intactness maps

  - 09_prep_valid_data.R
  - 10_clip_intact_maps.R
  - 11_sum_bead_errors.R
