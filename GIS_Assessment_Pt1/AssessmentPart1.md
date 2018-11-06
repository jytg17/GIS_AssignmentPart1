AssessmentPart1
================
Joshua Yee
5 November 2018

The genesis of any map is rooted in the specific agenda that it is meant to achieve. It is argued that clarifying one's objectives is fundamental to the practice of developing maps as it defines the subsequent processes of data identification and content representation (Harley, 1989; Krygier and Wood, 2016).

Map 1 was conceived from the objective of highlighting areas where concentrations of the urban poor are disadvantaged by low levels of access to public transportation in London. Map 1 therefore made use of TfL's Public Transport Accessibility Level (PTAL) scores and data on income deprivation collated by government sources, as they were relevant indicators reflecting the real-world phenomena of interest and the data had been aggregated according to widely-used statistical boundaries. To maximise its utility, both datasets should ideally be overlaid with one another, and hence a bi-variate choropleth map was chosen as the medium of representation.

**Map 1: Bi-variate Choropleth Map highlighting areas with their density of income deprived individuals and corresponding PTAL scores** <img src="N:/GIS_code/GIS_Assessment_Pt1/Maps/assignment_lr.png" width="9934" />

In comparison, map 2 was driven by the inspiration to understand the spatial distribution of pubs in Great Britain with precision. While using data aggregated by area and presentations through choropleth maps were possibilities, there would be trade-offs with the level of spatial resolution sought for this map. Eventually, a dataset containing all pubs and their attributes as individual data points was obtained. It allowed for the mapping of pubs individually and visualising them as dot-density maps.

**Map 2: Dot-density Map showing the spatial distribution of open pubs in Great Britain** <img src="N:/GIS_code/GIS_Assessment_Pt1/Maps/Map 2_GIS assignment_R.png" width="5492" />

Heeding Guelke's (2011) call to consider the meanings communicated in our maps, upfront planning with regard to data presentation was done to ensure that the intended message could be optimally conveyed without misinterpretations. This step was particularly important for Map 1 given the inherent limitations in working with data tied to non-uniform boundaries (Krygier and Wood, 2016). Consequently, deliberate efforts were made to obtain data layers with some level of granularity and homogeneity (Boscoe and Pickle, 2003). From the boundaries available, the Lower Super Output Areas (LSOA) were chosen as the scale to represent nuances of the data in Map 1. Additionally, as the income deprivation data was available only as absolute counts tagged to LSOAs, transformations were applied to the figures to derive rates that allowed quantitative comparisons to be made (Krygier and Wood, 2016).

Critiquing the final products, both maps can generally be considered to achieve its original purposes. A perceiver would be able to single out LSOAs with concentrations of income deprivation coinciding with poor public transport accessibility from Map 1, while the spatial clustering patterns of pubs in Great Britain can be observed in Map 2. However, imperfections with the maps are acknowledged. For instance, while displaying the nuances of spatial data in 9 different classes on Map 1 augments the richness of detail, it could be perceived as over-complicated and hinder interpretation. With both static maps compacting in multiple layers of information presented at broad scales, it entails challenges in incorporating additional features like city or street names to aid orientation. However, this draw-back could be addressed with the use of digital maps that allows the zooming into smaller scales.

**Map 2a: Screengrab of the interactive Dot-density Map focusing on the spread of pubs in London, as a subset of the larger Great Britain dataset.Refer to link: <http://rpubs.com/jytg17/436421> for actual interactive map.** <img src="N:/GIS_code/GIS_Assessment_Pt1/Maps/Interactive_screengrab.png" width="1366" />

While both maps could technically be done on ArcGIS and R, the execution on each platform involved varying levels of ease depending on the nature and workflows required of the maps. With the bi-variate choropleth map, greater considerations were given to the content styling to harmonise the colours, line weights and micro-features of the map so that the message would be apparent. Hence, the ability for users to to select and preview from a comprehensive array of styling options on ArcGIS' GUI-interface was handy. Nonetheless, for the dot-density map which necessitated a constant review and re-execution of steps in the workflow, the use and reproducibility of code in R facilitated this process conveniently (Lovelace et al., 2018; Singleton et al., 2016). Furthermore, the seamlessness of pulling in online base plans and creating interactive maps boosted R's utility in creating this map in both static and digital versions.

**Bibliography** (Boscoe and Pickle 2003; Guelke 2011; Harley 1989; Krygier and Wood 2016; Lovelace, Nowosad, and Muenchow 2018; Singleton, Spielman, and Brunsdon 2016)

Boscoe, Francis P., and Linda W. Pickle. 2003. “Choosing Geographic Units for Choropleth Rate Maps, with an Emphasis on Public Health Applications.” *Cartography and Geographic Information Science* 30 (3): 237–48. doi:[10.1559/152304003100011171](https://doi.org/10.1559/152304003100011171).

Guelke, Leonard. 2011. “Cartographic Communication and Geographic Understanding.” *Classics in Cartography*, Wiley Online Books,, March. doi:[10.1002/9780470669488.ch10](https://doi.org/10.1002/9780470669488.ch10).

Harley, J. B. 1989. “Deconstructing the Map.” *Cartographica: The International Journal for Geographic Information and Geovisualization* 26 (2): 1–20.

Krygier, John, and Denis Wood. 2016. *Making Maps: A Visual Guide to Map Design for GIS*. Third edition. New York: Guilford Press.

Lovelace, Robin, Jakub Nowosad, and Jannes Muenchow. 2018. “Introduction.” *Geocomputation with R*. <https://bookdown.org/robinlovelace/geocompr/>.

Singleton, Alex David, Seth Spielman, and Chris Brunsdon. 2016. “Establishing a Framework for Open Geographic Information Science.” *International Journal of Geographical Information Science* 30 (8): 1507–21. doi:[10.1080/13658816.2015.1137579](https://doi.org/10.1080/13658816.2015.1137579).
