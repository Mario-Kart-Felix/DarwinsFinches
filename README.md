# Darwin's Finches
Statistical analysis on [''40 years of evolution. Darwin's finches on Daphne Major Island''](https://doi.org/10.5061/dryad.g6g3h). This analysis was part of [DataCamp's statistical thinking course](https://campus.datacamp.com/courses/statistical-thinking-in-python-part-2/). Results show introgressive hybridization of two finch species on Daphne Major. 

## Table of Contents
* [References](#refs)
* [Requirements](#libs)
* [Abstract](#abstract)
* [Methods](#methods)
    * Exploratory Data Analysis
    * Parameter Estimation
    * Hypothesis Testing
* [Discussion](#discuss)


## References <a class="anchor" id="refs"></a>
1. Grant, Peter R.; Grant, B. Rosemary (2013), Data from: 40 years of evolution. Darwin's finches on Daphne Major Island, Dryad, Dataset, https://doi.org/10.5061/dryad.g6g3h
2. Grant, Peter R, and B Rosemary Grant. “The Secondary Contact Phase of Allopatric Speciation in Darwin&#039;s Finches.” Proceedings of the National Academy of Sciences 106, no. 48 (December 1, 2009): 20141 LP – 20148. https://doi.org/10.1073/pnas.0911761106.
3. [DataCamp - Statistical Thinking in Python Part 2](https://campus.datacamp.com/courses/statistical-thinking-in-python-part-2/).

## Requirements <a class="anchor" id="libs"></a>
* [pandas](https://pandas.pydata.org/)
* [urllib](https://docs.python.org/3/library/urllib.html)
* [Matplotlib](https://matplotlib.org/)
* [seaborn](https://seaborn.pydata.org/)
* [NumPy](https://numpy.org/)

## Abstract <a class="anchor" id="abstract"></a>
In 1981 an immigrant finch species of medium size (Geospiza fortis) moved onto the island of Daphne Major. Peter and Rosemary Grant documented the lineage of the Geospiza scandens and Geospiza fortis for roughly 40 years. Their [publication](https://doi.org/10.1073/pnas.0911761106) on the results suggest introgressive hybridization. Here we analyze the [Grant's data](https://doi.org/10.5061/dryad.g6g3h) to determine if the beak shape of Geospiza scandens has changed. Results indicate a beak shape change that is consistent with introgressive hybridization. 

## Methods <a class="anchor" id="methods"></a>
Performed EDA, parameter estimation, and hypothesis testing on G. scandens (beak length and beak width). 
* EDA
   ECDF of beak length and beak depth for Geospiza scandens from 1975 and 2012.
   ![BeakLength-EDA](/images/beaklength_eda.png)
   ![BeakDepth-EDA](/images/depth_eda.png)

* Parameter Estimation
Bootstrap replicates (100k) of beak length and beak depth for Geospiza scandens.
  * Beak Length 95% CI [0.498102, 0.90263834] mm
  * Beak Depth 95% CI [-0.39105464, -0.06013981] mm

* Hypothesis Test
Bootstrap replicates (100k) to calculate p-values for changes in beak length and beak depth for Geospiza scandens.
  * Beak Length p = 0.000000
  * Beak Depth p = 0.996470

## Discussion <a class="anchor" id="discuss"></a>
Results suggest that Geospiza scandens beaks have grown deeper and shorter. Additional analysis of beak variation and heritability suggest stronger heritability with Geospiza fortis offspring. In conclusion, these results support the Grant's findings of introgressive hybridization. 
    
    

