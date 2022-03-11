# ANÁLISE DE DADOS DE ACIDENTES DE TRÂNSITO DA POLÍCIA RODOVIÁRIA FEDERAL NO PERÍODO DE 2017 A 2019

Repositório contendo código-fonte para realização de Projeto de Graduação 2 do aluno Gustavo Fardin Monti, do Curso de Engenharia da Computação (CEUNES).

## Como utilizar este repositório

Por favor, clone o repositório. Caso você nunca tenha clonado algo de um repositório, [confira este tutorial](https://docs.github.com/pt/repositories/creating-and-managing-repositories/cloning-a-repository).

O arquivo **relatório.html** pode ser visualizado com qualquer navegador. Por ser um arquivo R Markdown, qualquer parte do código utilizado para produzir as visualizações e transformações pode ser visualizado através do collapse. Note a presença de um botão chamado "CODE" no canto superior direito da tabela, e também próximo as visualizações e blocos de saída de código. Estes botões podem ser utilizados para mostrar e esconder o código-fonte por trás da saída. 

![alt text](Images/demo_relatorio.gif)

Caso você queira, você também pode explorar os mapas interativos criados de dados acidentes. Estes gráficos foram separados do relatório principal devido ao tamanho dos arquivos. Há dois tipos principais de mapas:
- Mapa de calor: Mapa interativo que permite visualizar os acidentes como pontos no mapa. Uma grande concentração de acidentes é representado pela cor vermelha. Os circulos com numero representam agrupmentos de acidentes. Um exemplo pode ser visto no GIF abaixo.
- Mapa coroplético: Mapa interativo que mostra o numero de acidentes por unidade federativa.

Para os  dois tipos de mapas, há um arquivo para cada ano.

![alt text](Images/demo_mapa.gif)

Caso queira explorar o código-fonte por trás deste arquivo, favor abrir o arquivo **relatório.Rmd** através do RStudio. 

![alt text](Images/demo_rstudio.gif)

## Organização de Arquivos

📦**tcc2-kdd-prf**: Raiz do repositório. \
 ┣ 📂**Base de Dados**: Fonte de dados na forma crua. \
 ┣ 📂**Mapas Leaflet**: Mapas interativos gerados durante a análise exploratória. \
 ┣ 📜**BRUFE250GC_SIR.cpg**: Dados de contorno utilizados para gerar mapas. \
 ┣ 📜**BRUFE250GC_SIR.dbf**: Dados de contorno utilizados para gerar mapas. \
 ┣ 📜**BRUFE250GC_SIR.prj**: Dados de contorno utilizados para gerar mapas. \
 ┣ 📜**BRUFE250GC_SIR.shp**: Dados de contorno utilizados para gerar mapas. \
 ┣ 📜**BRUFE250GC_SIR.shx**: Dados de contorno utilizados para gerar mapas. \
 ┣ 📜**dadosSessao.RData**: Variáveis da sessão RStudio exportadas. \
 ┣ 📜**README.md**: Este arquivo. \
 ┣ 📜**ref.bib**: Arquivo de referências para o relatório. \
 ┣ 📜**relatorio.html**: Relatório compilado. Visualizar com um navegador. \
 ┣ 📜**relatorio.Rmd**: Código Fonte/Notebook do relatório. \
 ┗ 📜**TCC2.pdf**: Projeto de graduação.

 ## Dependências

 A lista de dependências (incluindo a versão do RStudio) pode ser visualizadas através do Relatório compilado. Abaixo, anexou-se uma cópia:

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