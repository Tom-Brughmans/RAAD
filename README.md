# RAAD

This archive includes the data, notebooks, and figures to replicate and reuse the data analysis of Roman Amphorae in Germania published as:

Franconi, T. V., T. Brughmans, E. Borisova & L. Paulsen. From Empire-wide integration to regional localization: A synthetic and quantitative study of heterogeneous amphora data in Roman Germania reveals centuries-long change in regional patterns of production and consumption. PloS one.

Data:

The dataset used directly in all data analysis and to create the figures is RAAD_data_restructured.csv (located in: RAAD/RAAD_data/data).

This is tabular data in which each row represents one unique combination of an amphora type (RAAD_type_number), found at a site (site_number) in a certain frequency (frequency).

<b>Field Name:          Type /	Description</b>

'RAAD_form'	        string /	Commonly used typologies for RAAD type number

'RAAD_type_number'	integer /	RAAD unique form identifier

'origin'	          string /	A region where an amphora was produced 

'origin_h1'	        string /	A region where an amphora was produced 

'origin_h2'	        string /	A subregion of a region (where an amphora was made) 

'contents'	        string /	A product carried in an amphora 

'site_name_modern'	string /	A modern name of an archaeological site from which an amphorae assemblage came 

'site_name_ancient' 	string /	Roman name for sites (where known)

'site_number'	integer /	RAAD unique assemblage identifier

'modern_country' 	string /	Modern national location of sites

'roman_province'	string /	Ancient provincial location of sites

'major_site_type'	string /	A site category: 1.	military, 2.	settlement, 3.	oppidum , 4.	villa

'minor_site_type' 	string /	Specific types of sites, where available

'quantification_method'	string /	The method with which each assemblage was quantified

'quantification_abbreviation'	string /	A ceramic quantification method:1.	total - total sherd count, 2.	mni - minimum number of individuals, 3.	rbh - diagnostic rim, base, and handles count , 4.	max - maximum number of individuals

'raad_type_start_date'	float /	A production start date of an amphora

'raad_type_end_date'	float /	A production end date of an amphora

'site_start_date'	integer /	A consumption start date of an amphora

'site_end_date'	integer /	A consumption end date of an amphora

'frequency'	integer /	An amphora frequency 

'southampton_type_number' 	float /	Corresponding entry in Southampton Roman Amphorae: a Digital Resource (if available)

'pleiades'	float /	Site geographical coordinates according to the Pleiades Atlas

'dare'	float /	Site geographical coordinates according to the Digital Atlas of the Roman Empire

'vici'	float /	Site geographical coordinates according to the Archaeological Atlas of Antiquity

'lat'	float /	Site geographical coordinates in latitude

'long'	float /	Site geographical coordinates in longitude

'total assemblage size' 	integer /	Total number of amphorae/sherds per site

'reference'	string /	Bibliographic reference for assemblage publication


Notebooks:


Figures:


Abstract of study:

We present novel insights into trade in amphorae-borne products over a 550-year period in Germania along the frontier of the Roman Empire, derived through probabilistic aoristic methods to study temporal changes in archaeological materials. Our data analysis reveals highly detailed differential patterns of consumption and production within the German market. We show how connections to far-flung regions such as the Eastern Mediterranean or the Iberian Peninsula wax and wane through time, and how the local German producers start to compete with these imported products. These chronological patterns provide important insight into a regional market within the larger Roman economy and provide an important case study in changing economic connections over a long period, demonstrating in a transparent and reproducible way a geographical and chronological pulsation in market activity that was otherwise unknown and undemonstrated.

Funding and acknowledgements:

TF, John Fell Oxford University Press (OUP) Research Fund, (BED12620, 153/058). https://researchsupport.admin.ox.ac.uk/funding/internal/jff.

TB, Danmarks Frie Forskningsfond (DFF) Sapere Aude research leadership grant (0163-00060B). https://dff.dk/en/grants?set_language=en .

TB, Past Social Networks Project was funded by The Carlsberg Foundation’s Young Researcher Fellowship (CF21-0382). https://www.carlsbergfondet.dk/en/Forskningsaktiviteter/Bevillingsstatistik/Bevillingsoversigt?type=Carlsberg%20Foundation%20Young%20Researcher%20Fellowships.

The funders had no role in study design, data collection and analysis, decision to publish, or preparation of the manuscript.
