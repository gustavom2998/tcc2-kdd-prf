# ANALYSIS OF TRAFFIC ACCIDENT DATA FROM THE FEDERAL HIGHWAY POLICE DATASET FROM 2017 TO 2019

English (EN) | [Português (PT-BR)](./README-pt.md)

Repository containing source code for the student Gustavo Fardin Monti's Undergraduate thesis for his BE in Computer Engineering at the Federal University of Espirito Santo (UFES).

## Thesis Summary

With its continental dimensions, Brazil is a country with a great highway network, responsible for integrating the country by allowing the movement and transport of merchandise. However, due to its large extension and high traffic of vehicles, the highway network has an abundant number of accidents that inspires research. The objective of this study was to find patterns between attributes of the road-traffic accident database grouped by individuals of the Federal Highway Police corresponding to the years 2017 to 2019 to understand the factors that influence the profile of a road traffic accident victim. The process of Knowledge Discovery in Databases was applied to the public database. The R programming language and the RStudio tool were used to execute the necessary steps for this study. The steps of Pre-processing and Exploratory Analysis were executed simultaneously. In the data mining step, the Apriori algorithm was used, resulting in a set of association rules for each value of the columns of interest (Sex, Physical State, and Involvement), thereby producing approximately 50 rules per attribute-value pair with confidence larger than 0,8 and lift larger than 1,2. The results obtained by applying the Apriori algorithm were rules with confidence greater than 0,8 and lift greater than 1,2. Using the R programming language, we applied the process of Knowledge Discovery to the Federal Highway Police data set in order to generate association rules. By interpreting the rules, our findings are: A significant part of the dataset is comprised of male, uninjured drivers; Passengers are associated with female individuals who sustained minor injuries; Pedestrians are associated with more severe injuries; Witnesses are associated with missing values.

## How to use this repository

Please clone this repository locally. In case you have never done this, check out the following [tutorial](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).

The file [`relatorio.html`](./relatorio.html) can be viewed with any web browser. Being an R Markdown file, any part of the code used to generate visualizations and transformations can be viewed using the collapse feature. Notice the presence of a button called "CODE" in the upper right corner of the table, as well as next to the visualizations and code output blocks. These buttons can be used to show and hide the source code responsible for the output.

![alt text](Images/demo_relatorio.gif)

If you wish to, you can also explore the [folder](./Mapas%20Leaflet/) containing the interactive maps created from accident data. These graphics have been separated from the main report due to file size. There are two main types of maps:

- [Heatmap](./Mapas%20Leaflet/mapa2017.html): An interactive map that allows you to visualize accidents as points on the map. A high concentration of accidents is represented by the color red. Circles with numbers represent clusters of accidents. An example can be seen in the GIF below.
- [Choropleth Map](./Mapas%20Leaflet/mapaUF2017.html): An interactive map that displays the number of accidents per federal unit.

For the two types of maps, there is a file for each year of data.

![alt text](Images/demo_mapa.gif)

In case you want to see the source code behind the rendered markdown notebook, please check the file `relatório.Rmd` in RStudio.

![alt text](Images/demo_rstudio.gif)

## File tree

📦**tcc2-kdd-prf**: \
 ┣ 📂**Base de Dados**: Raw data source. \
 ┣ 📂**Mapas Leaflet**: Interactive maps generated during the analysis. \
 ┣ 📜**BRUFE250GC_SIR.cpg**: Contour data used to generate maps. \
 ┣ 📜**BRUFE250GC_SIR.dbf**: Contour data used to generate maps. \
 ┣ 📜**BRUFE250GC_SIR.prj**: Contour data used to generate maps. \
 ┣ 📜**BRUFE250GC_SIR.shp**: Contour data used to generate maps. \
 ┣ 📜**BRUFE250GC_SIR.shx**: Contour data used to generate maps. \
 ┣ 📜**dadosSessao.RData**: Exported RStudio session containing Variables. \
 ┣ 📜**README.md**: This file. \
 ┣ 📜**README-pt.md**: This file in Portuguese. \
 ┣ 📜**ref.bib**: Bibliographical references used for the report. \
 ┣ 📜**relatorio.html**: Rendered markdown file. \
 ┣ 📜**relatorio.Rmd**: Source code for markdown file. \
 ┗ 📜**TCC2.pdf**: Undergraduate thesis PDF.

 ## Dependencies

The following lists includes the dependencies (include the RStudio version) used to build the report.

```R
## R version 3.6.2 (2019-12-12)
## Platform: x86_64-w64-mingw32/x64 (64-bit)
## Running under: Windows 10 x64 (build 19043)
## 
## Matrix products: default
## 
## locale:
## [1] LC_COLLATE=Portuguese_Brazil.1252  LC_CTYPE=Portuguese_Brazil.1252   
## [3] LC_MONETARY=Portuguese_Brazil.1252 LC_NUMERIC=C                      
## [5] LC_TIME=Portuguese_Brazil.1252    
## 
## attached base packages:
## [1] grid      stats     graphics  grDevices utils     datasets  methods  
## [8] base     
## 
## other attached packages:
##  [1] lubridate_1.7.4      kableExtra_1.1.0     viridis_0.5.1       
##  [4] viridisLite_0.3.0    wordcloud_2.6        RColorBrewer_1.1-2  
##  [7] knitr_1.28           magrittr_1.5         dplyr_0.8.4         
## [10] leaflet.extras_1.0.0 sp_1.3-2             leaflet_2.0.3       
## [13] plotly_4.9.2         ggplot2_3.3.0        arulesViz_1.3-3     
## [16] arules_1.6-4         Matrix_1.2-18        DT_0.13             
## 
## loaded via a namespace (and not attached):
##  [1] bitops_1.0-6         webshot_0.5.2        httr_1.4.1          
##  [4] tools_3.6.2          R6_2.4.1             KernSmooth_2.23-16  
##  [7] lazyeval_0.2.2       colorspace_1.4-1     withr_2.1.2         
## [10] tidyselect_1.0.0     gridExtra_2.3        compiler_3.6.2      
## [13] rvest_0.3.5          TSP_1.1-8            NLP_0.2-0           
## [16] xml2_1.2.2           slam_0.1-47          labeling_0.3        
## [19] bookdown_0.18        caTools_1.18.0       scales_1.1.0        
## [22] tm_0.7-7             lmtest_0.9-37        readr_1.3.1         
## [25] stringr_1.4.0        digest_0.6.25        rmarkdown_2.1       
## [28] pkgconfig_2.0.3      htmltools_0.4.0      fastmap_1.0.1       
## [31] htmlwidgets_1.5.1    rlang_0.4.4          rstudioapi_0.11     
## [34] shiny_1.4.0          visNetwork_2.0.9     farver_2.0.3        
## [37] zoo_1.8-7            jsonlite_1.6.1       crosstalk_1.0.0     
## [40] gtools_3.8.1         dendextend_1.13.3    Rcpp_1.0.3          
## [43] munsell_0.5.0        lifecycle_0.1.0      scatterplot3d_0.3-41
## [46] stringi_1.4.4        yaml_2.2.1           MASS_7.3-51.5       
## [49] gplots_3.0.1.2       parallel_3.6.2       gdata_2.18.0        
## [52] promises_1.1.0       crayon_1.3.4         lattice_0.20-38     
## [55] hms_0.5.3            pillar_1.4.3         igraph_1.2.4.2      
## [58] codetools_0.2-16     glue_1.3.1           gclus_1.3.2         
## [61] evaluate_0.14        data.table_1.12.8    vcd_1.4-5           
## [64] vctrs_0.2.2          rmdformats_0.3.7     httpuv_1.5.2        
## [67] foreach_1.4.8        gtable_0.3.0         purrr_0.3.3         
## [70] tidyr_1.0.2          assertthat_0.2.1     xfun_0.12           
## [73] mime_0.9             xtable_1.8-4         later_1.0.0         
## [76] seriation_1.2-8      tibble_2.1.3         iterators_1.0.12    
## [79] registry_0.5-1       cluster_2.1.0
```