# RAAD

<b>This archive includes the data, notebooks, and figures to replicate and reuse the data analysis of Roman Amphorae in Germania published as:</b>

[Franconi, T. V., T. Brughmans, E. Borisova & L. Paulsen. *From Empire-wide integration to regional localization: A synthetic and quantitative study of heterogeneous amphora data in Roman Germania reveals centuries-long change in regional patterns of production and consumption*. PloS one.](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0279382)

# Contributors

The notebooks are developed in collaboration with the [Center for Humanities Computing Aarhus (CHCAA)](https://chcaa.io/#/).

* [Ekaterina S. Borisova](https://github.com/esborisova)
* [Laura B. Paulsen](https://github.com/laurabpaulsen)
* [Peter B. Vahlstrup](https://pure.au.dk/portal/en/persons/peter-bjerregaard-vahlstrup(63997fd6-cf3c-4d7e-895a-7cfbd145f22e).html)
* [Kristoffer L. Nielbo](https://pure.au.dk/portal/en/persons/kristoffer-laigaard-nielbo(aef8887c-d4e9-4270-9031-1a15553f5590).html)
* [Tom Brughmans](https://pure.au.dk/portal/en/persons/tom-brughmans(78c7314a-9485-4e14-b207-0e836aea5e01).html)
* [Tyler V. Franconi](https://www.brown.edu/academics/archaeology/people/franconi)

# Data

The dataset used directly in all data analysis and to create the figures is RAAD_data_restructured.csv (located [here](https://github.com/Tom-Brughmans/RAAD/tree/main/RAAD_data/data)).

This is tabular data in which each row represents one unique combination of an amphora type (RAAD_type_number), found at a site (site_number) in a certain frequency (frequency).
<br /> 

<details>
  <summary>  The data table </summary>

|**Field Name**                |      **Type / Description**                                                                      |
| ---------------------------- | ---------------------------------------------------------------------------------------------- |
|'RAAD_form'	               |   string / Commonly used typologies for RAAD type number                                         |
|'RAAD_type_number'            |   integer / RAAD unique form identifier                                                          |
|'origin'               	   |   string / A region where an amphora was produced                                                |
|'origin_h1'	               |   string / A region where an amphora was produced                                                |
|'origin_h2'	               |   string / A subregion of a region (where an amphora was made)                                   |
|'contents'	                   |   string / A product carried in an amphora                                                       |
|'site_name_modern'	           |   string / A modern name of an archaeological site from which an amphorae assemblage came        |
|'site_name_ancient' 	       |   string / Roman name for sites (where known)                                                    |
|'site_number'                 |   integer / RAAD unique assemblage identifier                                                    |
|'modern_country'              |   string / Modern national location of sites                                                     |
|'roman_province'              |   string / Ancient provincial location of sites                                                  |
|'major_site_type'	           |   string / A site category: <ul><li>military</li><li>settlement</li><li>oppidum</li><li>villa</li></ul>|
|'minor_site_type'             |   string / Specific types of sites, where available                                              |
|'quantification_method'       |   string / The method with which each assemblage was quantified                                  |
|'quantification_abbreviation' |   string / A ceramic quantification method: <ul><li>total - total sherd count</li><li>mni - minimum number of individuals</li><li>rbh - diagnostic rim, base, and handles count</li><li>max - maximum number of individuals</li></ul>|
|'raad_type_start_date'        |   float / A production start date of an amphora                                                  |
|'raad_type_end_date'	       |   float / A production end date of an amphora                                                    |
|'site_start_date'	           |   integer / A consumption start date of an amphora                                               |
|'site_end_date'	           |   integer / A consumption end date of an amphora                                                 |
|'frequency'                   |   integer / An amphora frequency                                                                 |
|'southampton_type_number'     |   float / Corresponding entry in Southampton Roman Amphorae: a Digital Resource (if available)   |
|'pleiades'	                   |   float / Site geographical coordinates according to the Pleiades Atlas                          |
|'dare'    	                   |   float / Site geographical coordinates according to the Digital Atlas of the Roman Empire       |
|'vici'	                       |   float / Site geographical coordinates according to the Archaeological Atlas of Antiquity       |
|'lat'  	                   |   float / Site geographical coordinates in latitude                                              |
|'long'   	                   |   float / Site geographical coordinates in longitude                                             |
|'total assemblage size'       |   integer / Total number of amphorae/sherds per site                                             |
|'reference'	               |   string / Bibliographic reference for assemblage publication                                    |

</details>

<br /> 

## Original RAAD database

The version of the data used here is a restructured version of the original RAAD database collected by Tyler Franconi and openly available on Zenodo:

Franconi TV. Roman Amphorae Assemblages Database [Internet]. Zenodo; 2021 [cited 2022 Aug 21]. Available from: https://zenodo.org/record/5213724

Please cite this resource when citing the original RAAD dataset.

The original dataset is in a matrix format and includes multiple tables, which we restructured into a single table format to enable the data analysis of our study.


# Notebooks

The iPython notebooks used to generate all published data analysis figures are available [here](https://github.com/Tom-Brughmans/RAAD/tree/main/RAAD_data/publication).
RAAD/RAAD_data/publication/

Each notebook reproduces one figures, numbered in the same way as in the publication.

Each notebook is structured in the same way:

1. Import packages
2. Read in data: daring on the data in RAAD_data_restructured.csv
3. Data analysis queries: e.g. frequency of amphorae, count of sites, count of types
4. Plot the graphs

# Figures

The data analysis figures included in the publication are available [here](https://github.com/Tom-Brughmans/RAAD/tree/main/RAAD_data/publication/Figs).

# Abstract of study

We present novel insights into trade in amphorae-borne products over a 550-year period in Germania along the frontier of the Roman Empire, derived through probabilistic aoristic methods to study temporal changes in archaeological materials. Our data analysis reveals highly detailed differential patterns of consumption and production within the German market. We show how connections to far-flung regions such as the Eastern Mediterranean or the Iberian Peninsula wax and wane through time, and how the local German producers start to compete with these imported products. These chronological patterns provide important insight into a regional market within the larger Roman economy and provide an important case study in changing economic connections over a long period, demonstrating in a transparent and reproducible way a geographical and chronological pulsation in market activity that was otherwise unknown and undemonstrated.

# Funding and acknowledgements

TF, John Fell Oxford University Press (OUP) Research Fund, (BED12620, 153/058). https://researchsupport.admin.ox.ac.uk/funding/internal/jff.

TB, Danmarks Frie Forskningsfond (DFF) Sapere Aude research leadership grant (0163-00060B). https://dff.dk/en/grants?set_language=en .

TB, Past Social Networks Project was funded by The Carlsberg Foundation???s Young Researcher Fellowship (CF21-0382). https://www.carlsbergfondet.dk/en/Forskningsaktiviteter/Bevillingsstatistik/Bevillingsoversigt?type=Carlsberg%20Foundation%20Young%20Researcher%20Fellowships.

The funders had no role in study design, data collection and analysis, decision to publish, or preparation of the manuscript.

# Citing
```
@article{Franconi_2023,	doi = {10.1371/journal.pone.0279382},	
url = {https://doi.org/10.1371%2Fjournal.pone.0279382},	
year = 2023,	
month = {jan},	
publisher = {Public Library of Science ({PLoS})},	
volume = {18},	
number = {1},	
pages = {e0279382},	
author = {Tyler Franconi and Tom Brughmans and Ekaterina Borisova and Laura Paulsen},	
editor = {Fabio Gaetano Santeramo},	
title = {From Empire-wide integration to regional localization: A synthetic and quantitative study of heterogeneous amphora data in Roman Germania reveals centuries-long change in regional patterns of production and consumption},	
journal = {{PLOS} {ONE}}}
```
