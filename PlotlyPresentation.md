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
```{r echo=TRUE, eval=FALSE}
install.packages("plotly")
```
The source the library with:
```{r echo=TRUE}
library(plotly)
```

Showing a 3D scatterplot
========================================================
## Using the trees dataset
We will be using the trees dataset from R.
```{r echo=TRUE}
names(trees)
```

x: Girth  
y: Volume  
z: Height  


3D Scatterplot of tree data
========================================================

```{r, echo=TRUE}
library(plotly)

plot_ly(trees, x=~Girth,y=~Volume,z=~Height,type="scatter3d", 
        mode="markers", color=~Girth) %>%
	layout(
		scene = list(
			xaxis = list(title="Girth"),
			yaxis = list(title="Volume"),
			zaxis = list(title = "Height", titlefont = f)
		)
	)
```

Thank you
========================================================
