# Introduction to ecological modelling with `SpaDES`

This workshop assumes good familiarity with R as well as several of its contributed packages.

## Workshop content

0. Before the course ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-intro-00-prerequisites))

    - Set up your laptop
    - Set your goals for course
    - [all course material, zipped](https://github.com/PredictiveEcology/workshops/raw/master/SpaDES_intro.zip)

1. `SpaDES` in action (Eliot and Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-01-spades-in-action))

    - [The demo modules in the SpaDES package](https://github.com/PredictiveEcology/SpaDES/blob/master/inst/sampleModules/SpaDES_sampleModules/SpaDES_sampleModules.Rmd)
    - [LCC2005 model ("Land Cover Classification 2005")](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/LCC2005/LCC2005.html)
    - Vegetation simulation (SpaDES-Landis)
    - Agent based models – [wolf IBM](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/wolfAlps/wolfAlps.html)
    - A shiny app on shinyapps.io (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))
    
2. Thinking the `SpaDES` way (Eliot) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-02-thinking-the-spades-way))
    
    - Events
    
    - Modules
    
      - Types of `SpaDES` modules:
    
        - events (*e.g.*, Fire, Vegetation Change)
        - data preparation (*e.g.*, climate data downloading)
        - individual-based modules (*e.g.*, caribou, wolves, mountain pine beetle)
        - parents and children
    
    - Data

3.  Getting technical (Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-03-getting-technical))
    
    a. The parts
    
      - The [simList](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/.simList-class)
        
        - Modules
        - Events within modules
        - data
            
      - The [`spades`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/spades) call

    
    b. Surface dive
    
      - creating the `simList` ([`simInit()`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/simInit))
      - run model (`spades()`)
      - where to get help
      - using pre-built modules ([`downloadModule`]((http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/downloadModule)))
        

4. Building `SpaDES` modules (Alex) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-04-modules))
    
    a. new module template: [`newModule`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/newModule)
    
    b. module metadata [`defineModule`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/defineModule)
    
    c. scheduling events: [`scheduleEvent`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/scheduleEvent)
    
    d. [`time`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/time)
    
    e. visualizations: [`Plot`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/Plot)
    
    f. debugging (`spades(sim, debug = TRUE)`)
    
    g. [finding SpaDES tools](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/spades-package)
    
    h. [summary statistics](https://github.com/PredictiveEcology/SpaDES/wiki/Summary-statistics-in-simulations)

5. Simulation experiments and replication (Eliot) ([slides](http://Rpubs.com/PredictiveEcology/SpaDES-Intro-05-simulation-experiments-replication))
    
    a. using the `experiment()` function for replication, scenario creation, and parameter experiments
    
    b. running parallel simulations on supercomputers and clusters
    
    c. Pattern Oriented Modeling (`POM()` function) for estimating unknown parameters

6. Getting the most out of R for ecological models (Eliot and Alex)
    
    a. Spatial data (`raster` and `sp` packages)
    
    b. Matrices
    
    c. The `data.table` package
    
    d. `SpaDES` functions for spreading, moving, neighbourhoods etc. [section 2 of spades-package help file](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/spades-package)
    
    e. The `Rcpp` package
    
8. Module integration (Alex)
    
    a. Building "models", *i.e.*, groups of modules (parents and children)
    
    b. Using metadata
    
    c. Visual tools: [`objectDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/objectDiagram), [`moduleDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/moduleDiagram), [`eventDiagram`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0/topics/eventDiagram)

9. Sharing modules & models (Alex)
    
    a. `SpaDES` module repositories
    
    b. Using [GitHub.com](https://github.com)
    
    c. `shiny` apps and [shinyapps.io](http://www.shinyapps.io/) (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))
    
    d. Data sources

10. Data to decisions (Eliot)

    a. Building a reproducible workflow

    b. Caching
    

## Resources:

- [SpaDES wiki](https://github.com/PredictiveEcology/SpaDES/wiki)
- [R documentation for `SpaDES`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0)
- [Development release of `SpaDES`](https://github.com/PredictiveEcology/SpaDES/tree/development)

