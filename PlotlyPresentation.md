R Markdown Presentation & Plotly
========================================================
author: Glenn Kerbein
date: May 14, 2017
autosize: true

Instructions
========================================================

Create a web page presentation using R Markdown that features a plot created with Plotly. Host your webpage on either GitHub Pages, RPubs, or NeoCities. Your webpage must contain the date that you created the document, and it must contain a plot created with Plotly. We would love to see you show off your creativity!

## Required packages
Plotly
Can be installed with:

```r
install.packages("plotly"")
```
The source the library with:

```r
library(plotly)
```

Showing a 3D scatterplot
========================================================

We will be using the trees dataset from R.

```r
names(trees)
```

```
[1] "Girth"  "Height" "Volume"
```


Slide With Plot
========================================================

![plot of chunk unnamed-chunk-4](PlotlyPresentation-figure/unnamed-chunk-4-1.png)
