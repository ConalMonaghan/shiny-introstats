# Scatterplots 

This is a Shiny app that generates scatter diagrams using data about Climbing ropes.


## Motivation

The goal is to provide several examples of scatter diagrams with positive linear relations, negative linear relations, or non-linear relations, according to the material from __Statistics, Chapter 8: Correlation__

Reference: "Statistics" by David Freedman, Robert Pisani and Roger Purves (2007). Fourth Edition. Norton & Company.


## Data

This app uses one of my curated data sets about climbing (i.e. dynamic) ropes. The data is in the `ropes.txt` file which contains 101 rows and 6 columns: 

- `Name`: name of rope model
- `Brand`: brand name
- `Diameter`: diameter measured in mm
- `Weight`: weight measured in grams per meter 
- `Falls`: number of withstand [UIAA falls](http://www.rockandice.com/lates-news/Climb-Safe-fall-factors-explained)
- `ImpactForce`: [impact force](https://www.petzl.com/en/Sport/Fall-factor-and-impact-force---theory?ProductName=ARIAL-9-5-mm#.Vt-KFpMrL2Q)
- `StaticElongation`: percent of static [elongation](https://www.petzl.com/en/Sport/Elongation?ProductName=JAVA-10-3-mm#.Vt-KUZMrL2Q)
- `DynamicElongation`: percent of dynamic [elongation](https://www.petzl.com/en/Sport/Elongation?ProductName=JAVA-10-3-mm#.Vt-KUZMrL2Q)

The app does not uses variables: `Name, Brand`


## How to run it?

There are many ways to download the app and run it:

```R
library(shiny)

# Easiest way is to use runGitHub
runGitHub("shiny-introstats", "gastonstat", subdir = "scatterplot-ropes")
```

Or you can [clone](http://stackoverflow.com/questions/651038/how-do-you-clone-a-git-repository-into-a-specific-folder) the git repository, then use `runApp()`:

```R
# First clone the repository with git. If you have cloned it into
# ~/shiny-introstats, first go to that directory, then use runApp().
setwd("~/shiny-introstats/scatterplot-ropes")
runApp()
```
