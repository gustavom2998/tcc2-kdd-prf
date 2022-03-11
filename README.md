# ANÁLISE DE DADOS DE ACIDENTES DE TRÂNSITO DA POLÍCIA RODOVIÁRIA FEDERAL NO PERÍODO DE 2017 A 2019

Repositório contendo código fonte para realização de Projeto de Graduação 2.

## Como utilizar este repositório

Por favor clone o repositório. Caso você nunca tenha clonado algo de um repositório, [confira este tutorial](https://docs.github.com/pt/repositories/creating-and-managing-repositories/cloning-a-repository).

O arquivo **relatório.html** pode ser visualizado com qualquer navegador. Por ser um arquivo R Markdown, qualquer parte do código utilizado para produzir as visualizações e transformações pode ser visualizado através do collapse.

![alt text](Images/demo_relatorio.gif)

Caso você queira, você também pode explorar os mapas interativos criados de dados acidentes. Estes gráficos foram separados do relatório principal devido ao tamanho dos arquivos.

![alt text](Images/demo_mapa.gif)

Caso queira explorar o código fonte por trás deste arquivo, favor abrir o arquivo **relatório.Rmd** através do RStudio. A lista de depedências (incluindo a versão do RStudio) pode ser visualizadas através do Relatório compilado.

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
 ┣ 📜**dadosSessao.RData**: Váriaveis da sessão RStudio exportadas. \
 ┣ 📜**README.md**: Este arquivo. \
 ┣ 📜**ref.bib**: Arquivo de referências para o relatório. \
 ┣ 📜**relatorio.html**: Relatório compilado. Visualizar com um navegador. \
 ┣ 📜**relatorio.Rmd**: Código Fonte/Notebook do relatório. \
 ┗ 📜**TCC2.pdf**: Projeto de graduação.