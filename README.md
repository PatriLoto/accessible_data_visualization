# useR! 2022 - The R User Conference Online

\#\# Effective and Accessible Dataviz Workshop

![presentacion](https://raw.githubusercontent.com/PatriLoto/viz-datos-con-ggplot2-para-WIDS2020/master/presentacion_curso.png)

------------------------------------------------------------------------

## Fecha y Lugar

:spiral_calendar: June 23, 2022 :alarm_clock: 2 hours :hotel: Online

:earth_americas: [Más información sobre useR! 2022](https://user2022.r-project.org/)

### **A brief biography of the instructors**

-   **Patricia Loto**

Degree in Information Systems, Diploma in Data Science, Machine Learning and its Applications at the FAMAF belonging to the National University of Cordoba. Currently, I work as a software analyst and developer for the state lottery for the Province of Chaco in Argentina. In addition I analyzing data with R and SQL when the nature of the project requires it.analyzing data with R and SQL when the nature of the project requires it. My most recent project, where I am working with the Gambling Observatory, my main tasks are the generation of stored procedures (using SQL Server) and reports with Crystal Reports, as well as the detection of unusual betting patterns. I fervently believe that everything is better when we do it in a community, so I am part of several communities, I am co-founder and co-organizer of R-Ladies Resistencia - Corrientes, I am part of the accessibility team of Metadocencia since the beginning of 2021, and I have been part of the Organizing Committee of LatinR in 2019 and 2020. In addition, I am an instructor trained by The Carpentries and a member of DALAT (Latin American Accessible Development).

-   **Andrea Gomez Vargas**

Sociologist with orientation in Gender Studies and Human Rights. Currently I work as a Population Statistics Analyst at the National Institute of Statistics and Census in Argentina, and I am a university professor in feminist theory and data science. I have also participated in collaborative learning spaces in data science from the communities of R users in Argentina since 2019, and I am part of the organizing team of R-ladies Buenos Aires and LatinR. Professional website: <https://soyandrea.netlify.app/>

### **Abstract** 
There is a current demand for visualizations in data science that are understandable and can be accessed by a greater number of people. From this demand, the idea of this tutorial arises, which aims to be a brief learning guide to implement good practices of data visualization in R with a focus on accessibility.
We will start talking about the main best practices to make charts effective and reach the target audience and we will work with examples that will allow learners to understand the value of applying them. 
Regarding the accessibility axis, we will give a brief introduction about digital accessibility, and the principles of accessible design. We will teach with practical exercises in R how to apply these principles to data visualization in both static and dynamic graphs, using the ggplot2 and plotly libraries.
 

### ¿Este curso es para mí?

1.  Tienes conocimientos básicos del lenguaje R o Python y quieres aprender especificamente sobre visualización de datos.
2.  Quieres conocer cúales son los componentes visuales de un gráfico.
3.  Quieres entender los principios básicos de la Grámatica de gráficos en capas y cómo son implementadas en ggplot2.
4.  Quieres conocer cuáles son los gráficos más comúnmente utilizados y cómo desarrollarlos con ggplot2.

## :computer: Antes del workshop

Gracias por inscribirte a este workshop, en el mismo trabajaremos con la versión más reciente de R y Rstudio, por lo que, para aprovecharlo deberás traer una pc portátil con lo siguiente instalado:

### Instalación de R and RStudio

-   Una versión reciente de **R (\>=3.6.2)** disponible de manera gratuita para su descarga en [CRAN](https://cran.r-project.org/).

-   Una versión reciente de **Rstudio Desktop (\>=1.2.5033)** disponible de manera gratuita para su descarga en [Rstudio](https://www.rstudio.com/download).

En ambos casos, ten en cuenta cuál es el Sistema Operativo que utilizas y la versión del mismo (32 o 64 bits) para descargar la versión correcta tanto de R como de Rstudio.

-   Los paquetes que utilizaremos pueden instalarse, abriendo Rstudio y ejecutando las siguientes sentencias:

``` r
mis_paquetes <- c("tidyverse", "gapminder","babynames","survey","socviz","here","cowplot", 
                  "patchwork", "ggrepel","ggridges","ggforce", "gridExtra","extrafont",
                  "scales","wesanderson","viridis", "viridisLite","prismatic","fishualize",
                  "RColorBrewer","ggthemes","hrbrthemes","plotly","highcharter","GGally","sf",
                  "maps", "mapdata","mapproj","rnaturalearth","devtools")

install.packages(mis_paquetes, repos = "http://cran.rstudio.com")
remotes::install_github("clauswilke/ggtext")
```

Para poder instalar de manera exitosa los paquetes, es necesario que estés conectado a Internet.

### ¿Cómo verifico que los paquetes se instalaron correctamente?

Para verificar que los paquetes se cargaron correctamente, por favor ejecutá las sentencias que están a continuación:

``` r
easypackages::libraries("tidyverse", "gapminder","babynames","survey","socviz","here","cowplot", 
                        "patchwork", "ggrepel","ggridges","ggforce", "gridExtra","extrafont",
                        "scales","wesanderson","viridis", "viridisLite","prismatic","fishualize",
                        "RColorBrewer", "ggtext","ggthemes","hrbrthemes","plotly","highcharter","GGally",
                        "sf","maps", "mapdata","mapproj","rnaturalearth","devtools")
```

## :writing_hand: Slides y Código

Tanto la [presentación](https://github.com/PatriLoto/viz-datos-con-ggplot2-para-WIDS2020/blob/master/material/PRESENTACION_WIDS2020.pdf) como los [archivos rmarkdown](https://github.com/PatriLoto/viz-datos-con-ggplot2-para-WIDS2020/blob/master/material) se encuentran en la carpeta **Material**.

## :notebook: **Bibliografía**

Para la elaboración tanto del material teórico como de los ejercicios prácticos se utilizaron como referencia, los libros descriptos a continuación:

-   [R para Ciencia de Datos](https://es.r4ds.hadley.nz/) de Hadley Wickham - [Capítulo 3: Visualización de datos](https://es.r4ds.hadley.nz/visualizaci%C3%B3n-de-datos.html) y [Capítulo 28: Comunicar con gráficos](https://es.r4ds.hadley.nz/comunicar-con-gr%C3%A1ficos.html).

-   [R Graphics Cookbook: Practical Recipes for Visualizing Data](http://www.cookbook-r.com/Graphs/) de Winston Chang - [Capítulo 1: Bar and line graphs](http://www.cookbook-r.com/Graphs/Bar_and_line_graphs_(ggplot2)/).

-   [A Data Visualization: a practical introduction](http://socviz.co/) de [Kieran Healy](@kjhealy).

-   [Fundamentals of Data Visualization](https://serialmentor.com/dataviz/) de [Claus Wilke](@ClausWilke).

# **Material y Recursos Extras**

### :package: Paquetes

En el presente curso trabajaremos con el paquete ggplot2, pero existen otros paquetes que puedes explorar:

-   [patchwork](https://github.com/thomasp85/patchwork)/[cowplot](https://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html): tienen la misma finalidad, permiten combinar dos o más gráficos.

-   [paletteer](https://github.com/EmilHvitfeldt/paletteer): agrupa una gran colección de paletas de colores.

-   [plotly](https://plot.ly/r/)/[highcharter](http://jkunst.com/highcharter/index.html): ambos permiten realizar gráficos interactivos.

-   [gganimate](https://github.com/thomasp85/gganimate): permite agregarle animación a los gráficos hechos con ggplot2.

-   [esquisse](https://github.com/dreamRs/esquisse): facilita la exploración y visualización de datos.

-   [ggtext](https://github.com/wilkelab/ggtext): permite extender las funcionalidades de ggplot2, mediante la customización de títulos, subtítulos, anotaciones, etc.

Espero te sean de utilidad.

### :books: Libros para profundizar en la visualización de datos.

-   [ggplot2: Elegant Graphics for Data Analysis](https://ggplot2-book.org/) de [Hadley Wickham](@hadleywickham).

-   [Data Visualization with R](https://rkabacoff.github.io/datavis/) de Rob Kabacoff - [Capítulo 12: Interactive Graphs](https://rkabacoff.github.io/datavis/Interactive.html) y [Capítulo 13: Advice / Best Practices](https://rkabacoff.github.io/datavis/Advice.html).

-   [Graphical Data Analysis with R](http://www.gradaanwr.net/content/) de Antony Unwin.

### Sitios Webs.

-   [The R graph Gallery](https://www.r-graph-gallery.com/)
-   [Highcharter](http://jkunst.com/highcharter/)
-   [From Data to Viz](https://www.data-to-viz.com/)
-   [RStudio Education](https://rstudio.cloud/learn/primers/3)

### Tutoriales.

-   [A ggplot2 Tutorial for Beautiful Plotting in R](https://cedricscherer.netlify.com/2019/08/05/a-ggplot2-tutorial-for-beautiful-plotting-in-r/) por [Cédric Scherer](@CedScherer)

-   [The Grammar and Graphics of Data Science](https://rstudio.com/resources/additional-talks/the-grammar-and-graphics-of-data-science/) por Rstudio.

-   [Tutorial interactivo de gráficos con el paquete learnr](https://github.com/yabellini/tutorialgRaficosFN) por Yanina Bellini Saibene

### Presentaciones en español.

-   [Taller Introductorio a ggplot2](https://gabysandovalm.github.io/RLadiesChile_intro_ggplot/Presentacion_introggplot2#1) por [Gaby Sandoval](@GabySandovalM) para R-Ladies Santiago.
-   [Visualización de datos espaciales](https://sporella.github.io/datos_espaciales_presentacion/#1) por [Steph Orellana Bello](@sporella) para R-Ladies Santiago.

### Presentaciones en inglés.

-   [Take A Sad Plot & Make It Better](https://alison.netlify.app/uo-sad-plot-better/#1) por [Alison Presmanes Hill](@apreshill)
-   [Plot Twist: 10 Bake Offs, Visualized 11 Ways](https://alison.netlify.app/rls-plot-twist/#1) por [Alison Presmanes Hill](@apreshill)
-   [Data Visualization in the Tidyverse](https://alison.netlify.app/uo-tidy-bakeoff/#1) por [Alison Presmanes Hill](@apreshill)
-   [Data Visualisation in R](https://satrdayjoburg.djnavarro.net/slides) por [Danielle Navarro](@djnavarro)
-   [Robust-tools: data visualization](https://robust-tools.djnavarro.net/visualisation/) por [Danielle Navarro](@djnavarro)

### Talleres/Videos.

-   [Charlar con R - Toma 5 \| Visualizaciones y datos textuales para R-Ladies Bs-As.](https://www.youtube.com/watch?v=WXp1T9JEIRM) por [María Nanton](@bynans1)
-   [Drawing Anything with ggplot2](https://github.com/thomasp85/ggplot2_workshop) por Thomas Lin Pedersen.
-   [ggplot2 workshop part 1](https://www.youtube.com/watch?v=h29g21z0a68) por Thomas Lin Pedersen.
-   [ggplot2 workshop part 2](https://www.youtube.com/watch?v=0m4yywqNPVY) por Thomas Lin Pedersen.

### Para enseñar visualización de datos.

-   ["Let them eat cake (first)!"](https://github.com/mine-cetinkaya-rundel/eatcake) por [Mine Cetinkaya-Rundel](http://mine-cr.com)
-   [Incorporating visualization into statistics education](https://github.com/mine-cetinkaya-rundel/2016-03-04-viz-forum/blob/master/2016-03-04-viz-forum.pdf) por [Mine Cetinkaya-Rundel](http://mine-cr.com)
