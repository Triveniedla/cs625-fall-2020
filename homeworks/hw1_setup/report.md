Homework 1
================
Triveni Sangama Saraswathi

CS 625, Fall 2020

## Git, GitHub

1.  *What is your GitHub username?*
    
    Triveniedla

2.  *What is the URL of your remote GitHub repo (created through
    Mr. Kennedy’s exercises)?*
    
    <git@github.com>:Triveniedla/cs625-fall-2020.git

## R

The command below will load the tidyverse package. If you have installed
R, RStudio, and the tidyverse package, it should display a list of
loaded packages and their versions.

``` r
library(tidyverse)
```

    ## -- Attaching packages -------------------------------- tidyverse 1.3.0 --

    ## v ggplot2 3.3.2     v purrr   0.3.4
    ## v tibble  3.0.3     v dplyr   1.0.2
    ## v tidyr   1.1.2     v stringr 1.4.0
    ## v readr   1.3.1     v forcats 0.5.0

    ## -- Conflicts ----------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

## R Markdown

1.  *Create an ordered bulleted list with at least 3 items*

<!-- end list -->

  - Bulleted list item 1

  - Item 2
    
      - Item 2a
    
      - Item 2b

<!-- end list -->

2.  *Write a paragraph that demonstrates the use of italics, bold, bold
    italics, and code.*

3.  *Create an example of a fenced code block.*

4.  *Create a level 4 heading*

## R

#### Data Visualization Exercises

1.  *Run ggplot(data = mpg). What do you see?*
    
    ``` r
    'ggplot(data = mpg)'
    ```
    
        ## [1] "ggplot(data = mpg)"
    
    R is not showing any output.

2.  *How many rows are in mpg? How many columns?*
    
    There are 234 rows and 11 columns.

3.  *What does the drv variable describe? Read the help for ?mpg to find
    out.*
    
    It describes the type of drive train, where f=front-wheel drive,
    r=rear wheel drive, 4=4wd.

4.  *Make a scatterplot of hwy vs cyl.*
    
    ``` r
    ggplot(data = mpg) + 
      geom_point(mapping = aes(x = cyl, y = hwy))
    ```
    
    ![](report_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

5.  *What happens if you make a scatterplot of class vs drv? Why is the
    plot not useful?*

<!-- end list -->

``` r
ggplot(data = mpg) + 
 geom_point(mapping = aes(x = class, y = drv))
```

![](report_files/figure-gfm/unnamed-chunk-4-1.png)<!-- --> The
attributes class and drv are not showing any relationship.

#### Workflow: basics Exercises

1.  *Why does this code not work?*

<!-- end list -->

``` r
my_variable <- 10
my_varıable
```

2.  *Tweak each of the following R commands so that they run correctly:*

<!-- end list -->

``` r
library(tidyverse)

ggplot(data = mpg) + 
  geom_point(mapping = aes(x = displ, y = hwy))

fliter(mpg, cyl = 8)
filter(diamond, carat > 3)
```

3.  *Press Alt + Shift + K. What happens? How can you get to the same
    place using the menus?*

## Tableau

*Insert your the image of your final bar chart here*

1.  *What conclusions can you draw from the chart?*

## Observable and Vega-Lite

### A Taste of Observable

1.  *In the “New York City weather forecast” section, try replacing
    `Forecast: detailedForecast` with `Forecast: shortForecast`. Then
    press the blue play button or use Shift-Return to run your change.
    What happens?*

2.  *Under the scatterplot of temperature vs. name, try replacing
    `markCircle()` with `markSquare()`. Then press the blue play button
    or use Shift-Return to run your change. What happens? How about
    `markPoint()`?*

3.  *Under “Pick a location, see the weather forecast”, pick a location
    on the map. Where was the point you picked near?*

4.  *The last visualization on this page is a “fancy” weather chart
    embedded from another notebook. Click on the 3 dots next to that
    chart and choose ‘Download PNG’. Insert the PNG into your report.*

### Charting with Vega-Lite

1.  *Pass an option of { size: 200 } to markCircle().*

2.  *Try markSquare instead of markCircle.*

3.  *Try markPoint({ shape: ‘diamond’ }).*

4.  *Change Horsepower to Acceleration*

5.  *Swap what fields are displayed on the x- and y-axis*

6.  *Change Name to Origin.*

7.  *Remove the vl.y().fieldN(“Origin”) line.*

8.  *Replace count() with average(“Miles\_per\_Gallon”).*

## References

*Insert the list of sites you used as references as an unordered list
with named links here. This is required.*
