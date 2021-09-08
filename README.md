# Reprodutseeritav andmeanalüüs kasutades R keelt/Reproducible data analysis using R language

Eesmärgiks on, et kursusel osaleja oskaks hakata kasutada R keele tööriistu, selleks, et muuta oma toorandmed arusaamiseks ja teadmisteks. Kursusel õpetatakse kuidas andmeid importida, kuidas viia andmed sobiva kujuga tabelisse, tabelis olevaid andmeid summeerida, luua uusi muutujaid ja tulemusi visualiseerida kasutades `tidyverse` tööriistu.

The aim of the course is to learn how to start using R to turn raw data into insight and knowledge. You will learn how to import raw data to R, how to rearrange your data suitable for analysis, how to summarise and transform, how to visualise data using `tidyverse` R packages.

> If you have specific things you would like to learn to do in R, please let us know. Also, if you have specific problems with your datasets that you would like to solve, maybe we can do this in class as an excersise. If you have anything like that, we would appreciate if you write to us even this week, so that we can prepare this stuff for class.

## Tööriistad/Tools

Kursusel aktiivselt osalemiseks on vajalik:

- internetiühendusega süle**arvuti** olemasolu, kuhu on installeeritud
    - **R 4.1.0** (2021-05-18 -- "Camp Pontanezen") https://cran.r-project.org;      
    - **RStudio 1.4.1717** (desktop viimane versioon) https://www.rstudio.com/products/rstudio/download/;     
    - **git** https://git-scm.com/book/en/v2/Getting-Started-Installing-Git;     
- **_Github_ konto** https://github.com (jäta salasõna meelde!).


- You need to have following software available in your **computer**:
    - **R 4.1.0** (2021-05-18 -- "Camp Pontanezen") https://cran.r-project.org, 
    - **RStudio 1.4.1717** (desktop last version) https://www.rstudio.com/products/rstudio/download/, 
    - **git** https://git-scm.com/book/en/v2/Getting-Started-Installing-Git.
- **Github account** https://github.com (remember your password!).


### Required R packages/libraries

We are going to use following R libararies during the course:    

- **tidyverse** -- metapackage for easy install and load multiple 'tidyverse' packages in a single step, 
- **here** -- easy file paths by using the top-level directory of a file project, 
- **lubridate** -- work easier with dates and times,
- **cowplot** -- publication-quality figures with 'ggplot2',
- **reprex** -- create easy to share small reproducible examples.

As you can see there are lot's of 'easys', haha. If you manage to install them before course start then it's good (we can avoid mass tidyverse install during first session), but we will also show you how to install R packages in first session.           

All other packages will be installed when we need them.

These five packages can be installed by executing following code in R console:

``` r
install.packages(c("tidyverse", "here", "lubridate", "cowplot", "reprex"))
#> 
#> The downloaded binary packages are in
#>  /var/folders/tq/km9fzrbd0lxfddzznrhgyh000000gn/T//RtmpI01nyF/downloaded_packages
```

<sup>Created on 2021-09-01 by the [reprex package](https://reprex.tidyverse.org) (v2.0.0)</sup>

### Docker RStudio

Alternatively, you can start using containerized version of R and RStudio for much improved computational reproducibility. Follow [these instructions](Docker.md) how to get started with Docker and run dockerised RStudio server from your web browser. 

> Big plus is that e.g. 'rocker/verse' Docker container comes with preinstalled **tidyverse** packages.


## Programm/Program

Iga sessioon on jaotatud kaheks:
    - esimeses pooles vaatame süstemaatiliselt läbi *tidy* R andmeanalüüsi tööriistad ja 
    - teises pooles tegeleme praktilise andmeanalüüsiga.

Each session is divided into two parts,
    - in the first half, we go systematically through tidy R data analysis tools and
    - second half is dedicated to practical data analysis.

1) **Week 2, 7/9 Sep, 14.15-16.45**
    
    - Introduction, setting up RStudio workspace. How to search for R `?help`.
    - Introduction to base R.
    - Slight intro to version control (git + Github).
    - Data visualisation using **ggplot2**: components/layers of ggplot plot, scatterplots, aesthetics: color, size, shape.
    - Data visualisation using **ggplot2**: facetting, combining different types of geoms, plotting statistical summaries.

2) **Week 3, 14/16 Sep, 14.15-16.45**

    - Data transformation using five verbs from **dplyr** package. filter + logical operators and missing values, arrange rows, select columns, create new variables with mutate.
    - Data transformation using **dplyr** package: mutating and useful mutating functions.
    - How to use `%>%` (*pipe*) operator to compose data transformation sentences.

3) **Week 4, 21/23 Sep, 14.15-16.45**

    - Data grouping and grouped summaries,
    - Tidy data, formatting data frames/tibbles from wide to long format. Binding data frames by rows and columns and data frame merging by join-s. 

4) **Week 5, 28/30 Sep, 14.15-16.45**

    - Data import from from common file formats.
    - Data cleaning.

5) **Week 6, 5/7 Oct, 14.15-16.45**

    - Data types.
    - Iterating with map function, data frame list columns. Fitting linear models in tibble. Broom package.

6) **Week 7, 12/14 Oct, 14.15-16.45**

    - Groupwork: data analysis using provided dataset.

## Timing and location

> Classes will take place **14.15-16.45 on Tue in Ostwaldi 1 room A204 and on Thu in Nooruse 1 room 144**.

Week (acad. week) | Tue (Ostwaldi 1-A204) | Thu (Nooruse 1-144)
-------| ------------- | --------- 
36 (2) | 7 Sep.   | 9 Sep.
37 (3) | 14 Sep.  | 16 Sep.
38 (4) | 21 Sep.  | 23 Sep. 
39 (5) | 28 Sep.  | 30 Sep.
40 (6) | 5 Oct.   | 7 Oct.
41 (7) | 12 Oct.   | 14 Oct.
    
## Teachers:

**Ülo Maiväli, PhD**, associate professor, Institute of Technology, University of Tartu, Estonia. His research interests include applied Bayesian statistics, meta-science, and molecular biology of protein synthesis.

**Taavi Päll, PhD**, research fellow, Institute of Biological and Translational Medicine, University of Tartu, Estonia. His research interests include understanding the role of human gut virome in health and disease, computational reproducibility, applied Bayesian statistics. He is involved in Estonian Sars-Cov-2 sequencing project.

