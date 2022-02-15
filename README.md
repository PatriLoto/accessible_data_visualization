# useR! 2022 - The R User Conference Online

## Effective and Accessible Dataviz Workshop

------------------------------------------------------------------------

## Date

:alarm_clock: 2 hours :hotel: Online

:earth_americas: [More information about useR! 2022](https://user2022.r-project.org/)

### **A brief biography of the instructors**

-   **Patricia Loto**

Degree in Information Systems, Diploma in Data Science, Machine Learning and its Applications at the FAMAF belonging to the National University of Cordoba. Currently, I work as a software analyst and developer for the state lottery for the Province of Chaco in Argentina. In addition I analyzing data with R and SQL when the nature of the project requires it.analyzing data with R and SQL when the nature of the project requires it. My most recent project, where I am working with the Gambling Observatory, my main tasks are the generation of stored procedures (using SQL Server) and reports with Crystal Reports, as well as the detection of unusual betting patterns. I fervently believe that everything is better when we do it in a community, so I am part of several communities, I am co-founder and co-organizer of R-Ladies Resistencia - Corrientes, I am part of the accessibility team of Metadocencia since the beginning of 2021, and I have been part of the Organizing Committee of LatinR in 2019 and 2020. In addition, I am an instructor trained by The Carpentries and a member of DALAT (Latin American Accessible Development).

-   **Andrea Gomez Vargas**

Sociologist with orientation in Gender Studies and Human Rights. Currently I work as a Population Statistics Analyst at the National Institute of Statistics and Census in Argentina, and I am a university professor in feminist theory and data science. I have also participated in collaborative learning spaces in data science from the communities of R users in Argentina since 2019, and I am part of the organizing team of R-ladies Buenos Aires and LatinR. Professional website: <https://soyandrea.netlify.app/>

### **Abstract**

There is a current demand for visualizations in data science that are understandable and can be accessed by a greater number of people. From this demand, the idea of this tutorial arises, which aims to be a brief learning guide to implement good practices of data visualization in R with a focus on accessibility. We will start talking about the main best practices to make charts effective and reach the target audience and we will work with examples that will allow learners to understand the value of applying them. Regarding the accessibility axis, we will give a brief introduction about digital accessibility, and the principles of accessible design. We will teach with practical exercises in R how to apply these principles to data visualization in both static and dynamic graphs, using the ggplot2 and plotly libraries.

### **Intended audience and prerequisites:**

**Is this course for me?**

1.  You have initial knowledge of the R language and the ggplot2 and plotly packages, you make data visualizations with ggplot2 or Plotly and want to learn specifically about how to make your visualizations effective.
2.  You want to learn the basic principles of accessible design and how to implement them in your graphics.
3.  You want to learn what are best practices for visualizing data and making it accessible to more people.

**Prerequisites:**

**Before the tutorial.** To participate in this tutorial you need to have the latest version of R and Rstudio, here are the latest installation references: A recent version of R (\>=4.1.0) available for free download from CRAN. A recent version of Rstudio Desktop (\>= 2021.09.2+382) available for free download from Rstudio. In both cases, please note which Operating System you are using and the version of it (32-bit or 64-bit) to download the correct version of both R and Rstudio.

The packages we will use can be installed by opening Rstudio and executing the following statements:

``` r
mis_paquetes <- c("tidyverse", "gapminder","babynames","survey","here","cowplot", 
                  "patchwork", "ggrepel","ggridges","ggforce", "ggtext","gridExtra","extrafont",
                  "scales","wesanderson","viridis", "viridisLite","prismatic","fishualize",
                  "RColorBrewer","ggthemes","hrbrthemes","plotly","GGally","sf",
                  "maps", "mapdata","devtools")

install.packages(mis_paquetes, repos = "http://cran.rstudio.com")
```

In order to successfully install the packages, you need to be connected to the Internet.

### A brief outline of the tutorial\*\*\*\*

This is a 2-hour short course, in which the following topics will be covered:

| **Time (in minutes)** | **TOPICS**                                                                                                       |
|-----------------------|------------------------------------------------------------------------------------------------------------------|
| 15                    | **Presentation of the tutorial** (lecturers, main topics, working method)                                        |
| 25                    | **Axis 1 - Effective plots in R with ggplot2:**                                                                  |
|                       | \- Qualities of a good visualization. Practical examples.                                                        |
|                       | \- Good data visualization practices to generate effective plots with ggplot2 and plotly. Practical examples.    |
| 5                     | **Break 1**                                                                                                      |
| 25                    | **Axis 2 - Accessibility in data visualization:**                                                                |
|                       | \- Principles of accessibility and accessible design                                                             |
|                       | \- Accessible design applied to static and interactive graphics in R with ggplot2 and plotly. Practical examples |
| 5                     | **Break 2**                                                                                                      |
| 30                    | **Axis 3: Guided practice**                                                                                      |
| 10                    | **Final questions**                                                                                              |
| 5                     | **Survey and closing**                                                                                           |

## :writing_hand: Slides and Code

Both the [presentation]() like the [rmarkdown files](https://github.com/PatriLoto/viz-datos-con-ggplot2-para-WIDS2020/blob/master/material) they are located in the **Material** folder.

## :notebook: **Bibliography**

For the elaboration of both the theoretical material and the practical exercises, the books described below were used as reference:


* [An incomplete guide to accessible data visualization](https://towardsdatascience.com/an-incomplete-guide-to-accessible-data-visualization-33f15bfcc400)
* [Inclusive design](https://automattic.design/inclusive/)

*  [Accessible Visualization: Design Space, Opportunities, and Challenges](https://onlinelibrary.wiley.com/doi/abs/10.1111/cgf.14298)

* [Accessible colors for data visualization](https://zachgrosser.medium.com/accessible-colors-for-data-visualization-2ad64ac4ee7e)
* [A little book of accessibility](https://www.ab11y.com/articles/a-little-book-of-accessibility/)
* [How to design for accessibility](https://www.bbc.co.uk/gel/guidelines/how-to-design-for-accessibility)

-   [R for Data Science](https://es.r4ds.hadley.nz/) de Hadley Wickham - [Chapter 3](https://es.r4ds.hadley.nz/visualizaci%C3%B3n-de-datos.html) y [Chapter 28](https://es.r4ds.hadley.nz/comunicar-con-gr%C3%A1ficos.html).

-   [R Graphics Cookbook: Practical Recipes for Visualizing Data](http://www.cookbook-r.com/Graphs/) de Winston Chang - [Chapter 1 graphs](http://www.cookbook-r.com/Graphs/Bar_and_line_graphs_(ggplot2)/).

-   [A Data Visualization: a practical introduction](http://socviz.co/) de [Kieran Healy](@kjhealy).

-   [Fundamentals of Data Visualization](https://serialmentor.com/dataviz/) de [Claus Wilke](@ClausWilke).

## :package: **Packages**

-   [patchwork](https://github.com/thomasp85/patchwork)/[cowplot](https://cran.r-project.org/web/packages/cowplot/vignettes/introduction.html).

-   [paletteer](https://github.com/EmilHvitfeldt/paletteer).

-   [plotly](https://plot.ly/r/).

-   [gganimate](https://github.com/thomasp85/gganimate).

-   [esquisse](https://github.com/dreamRs/esquisse).

-   [ggtext](https://github.com/wilkelab/ggtext).


### :books: Books to delve into data visualization.

-   [ggplot2: Elegant Graphics for Data Analysis](https://ggplot2-book.org/) by [Hadley Wickham](@hadleywickham).

-   [Data Visualization with R](https://rkabacoff.github.io/datavis/) by Rob Kabacoff - [Capítulo 12: Interactive Graphs](https://rkabacoff.github.io/datavis/Interactive.html) and [Capítulo 13: Advice / Best Practices](https://rkabacoff.github.io/datavis/Advice.html).

-   [Graphical Data Analysis with R](http://www.gradaanwr.net/content/) by Antony Unwin.

### Webs.

-   [The R graph Gallery](https://www.r-graph-gallery.com/)
-   [Highcharter](http://jkunst.com/highcharter/)
-   [From Data to Viz](https://www.data-to-viz.com/)
-   [RStudio Education](https://rstudio.cloud/learn/primers/3)
