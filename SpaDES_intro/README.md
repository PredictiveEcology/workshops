# Introduction to ecological modelling with `SpaDES`

Alex M Chubaty & Eliot McIntire  

This workshop assumes good familiarity with R as well as several of its contributed packages.

# Dates and Times

**Dec 7-9, 2016 [google calendar link](https://calendar.google.com/calendar/event?action=TEMPLATE&tmeid=MzFvcDA5MmI3dDJhMDQxYTE4MzZpZDVuNW8gZWxpb3RtY2ludGlyZUBt&tmsrc=eliotmcintire%40gmail.com)**  
**8:30am - 4:30pm (PDT) each day**  
**Cost: Free**  
**Where: Pacific Forestry Centre, Victoria, BC**  
**WebEx: Limited numbers.** Contact Eliot.McIntire@canada.ca if you would like to participate remotely.  
**Rooms:** *TBD*  

# Workshop content 

([raw version of notes available on GitHub](https://github.com/PredictiveEcology/workshops/tree/master/SpaDES_intro))

## Before the course ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-intro-00-prerequisites))

- Set up your laptop
- Set your goals for course
- [all course material (incomplete until course begins), zipped](https://github.com/PredictiveEcology/workshops/raw/master/SpaDES_intro.zip)

## `SpaDES` in action (Eliot and Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-01-spades-in-action))

- [The demo modules in the `SpaDES` package](https://github.com/PredictiveEcology/SpaDES/blob/master/inst/sampleModules/SpaDES_sampleModules/SpaDES_sampleModules.Rmd)
- [LCC2005 model ("Land Cover Classification 2005")](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/LCC2005/LCC2005.html)
- Vegetation simulation (SpaDES-Landis)
- Agent based models – [wolf IBM](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/wolfAlps/wolfAlps.html)
- A shiny app on shinyapps.io (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))

## Thinking the `SpaDES` way (Eliot) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-02-thinking-the-spades-way))

- Events

- Modules

  - Types of `SpaDES` modules:

    - events (*e.g.*, Fire, Vegetation Change)
    - data preparation (*e.g.*, climate data downloading)
    - individual-based modules (*e.g.*, caribou, wolves, mountain pine beetle)
    - parents and children

- Data

## Getting technical (Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-03-getting-technical))
    
a. The parts
    
  - The [simList](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/.simList-class)
    
    - Modules
    - Events within modules
    - data
        
  - The [`spades`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/spades) call

    
b. Surface dive
    
  - creating the `simList` ([`simInit()`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/simInit))
  - run model (`spades()`)
  - where to get help
  - using pre-built modules ([`downloadModule`]((http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/downloadModule)))
        

## Building `SpaDES` modules (Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-04-modules))
    
a. anatomy of a `SpaDES` module
    
b. new module template: [`newModule`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/newModule)
    
c. module metadata [`defineModule`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/defineModule)
    
d. scheduling events: [`scheduleEvent`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/scheduleEvent)
    
e. [`time`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/time)
    
f. visualizations: [`Plot`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/Plot)
    
g. debugging (`spades(sim, debug = TRUE)`)
    
h. [finding SpaDES tools](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/spades-package)
    
i. [summary statistics](https://github.com/PredictiveEcology/SpaDES/wiki/Summary-statistics-in-simulations)
    
j. module development checklist

## Simulation experiments and replication (Eliot) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-05-simulation-experiments-replication))
    
a. using the `experiment()` function for replication, scenario creation, and parameter experiments
    
b. running parallel simulations on supercomputers and clusters
    
c. Pattern Oriented Modeling (`POM()` function) for estimating unknown parameters

## Getting the most out of R for ecological models (Eliot and Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-06-getting-most-out-of-r))

    
a. Spatial data (`raster` and `sp` packages)
    
b. Matrices
    
c. The `data.table` package
    
d. `SpaDES` functions for spreading, moving, neighbourhoods etc. [section 2 of spades-package help file](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/spades-package)
    
e. The `Rcpp` package
    
## Module integration (Alex)
([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-07-module-integration))
    
a. Building "models", *i.e.*, groups of modules (parents and children)
    
b. Using metadata
    
c. Visual tools: [`objectDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/objectDiagram), [`moduleDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/moduleDiagram), [`eventDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1/topics/eventDiagram)

## Sharing modules & models (Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-08-sharing-modules))
    
a. `SpaDES` module repositories
    
b. Using [GitHub.com](https://github.com)
    
c. `shiny` apps and [shinyapps.io](http://www.shinyapps.io/) (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))
    
d. Data sources

## Data to decisions (Eliot)
([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-09-workflow))

a. Building a reproducible workflow
b. Caching

# Resources

- [`SpaDES wiki`](https://github.com/PredictiveEcology/SpaDES/wiki)
- [R documentation for `SpaDES`](http://www.rdocumentation.org/packages/SpaDES/versions/1.3.1)
- [Development release of `SpaDES`](https://github.com/PredictiveEcology/SpaDES/tree/development)
- Link to this [Outline](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-Outline)
- Contact info: Eliot.McIntire@canada.ca or Alexander.Chubaty@canada.ca

# Archived content

Previous versions of this course are archived at the links below.

- [2016 Sept 14-16](http://rpubs.com/PredictiveEcology/Archives-Sept16-Outline)
