# Introduction to ecological modelling with `SpaDES`

This workshop assumes good familiarity with R as well as several of its contributed packages.

## Topics covered

1. What is `SpaDES`?
    
    a. how `SpaDES` works
    
        - modules
        - events
        - input and output objects
        - `simList` objects
    
    b. getting started with `SpaDES`
    
        - model specification (`simInit()` and `spades()`)
        - where to get help
        - using pre-built modules
    
    c. some more spohisticated examples
    
       - Fire (Beacons)
       - Vegetation simulation (SpaDES-Landis)
       - Agent based models – [wolf IBM](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/wolfAlps/wolfAlps.html)

2. Building `SpaDES` modules
    
    a. new module template: `newModule`
    
    b. module metadata
    
    c. scheduling events: `scheduleEvent`
    
    d. working with data
    
    e. visualizations
    
    f. summary statistics

3. Types of `SpaDES` modules
    
    a. events (*e.g.*, Fire)
    
    b. data preparation (*e.g.*, climate data downloading)
    
    c. individual-based modules (*e.g.*, caribou)

4. Simulation experiments and replication
    
    a. using the `experiment()` function for replication, scenario creation, and parameter experiments
    
    b. running parallel simulations on supercomputers and clusters
    
    c. Pattern Oriented Modeling (`POM()` function) for estimating unknown parameters

5. Getting the most out of R
    
    a. Spatial data (`raster` and `sp` packages)
    
    b. Matrices
    
    c. The `data.table` package
    
    d. The `Rcpp` package
    
    e. Other performance notes

6. Module integration
    
    a. Building "models", *i.e.*, groups of modules
    
    b. Parent modules and child modules

7. Sharing modules & models
    
    a. `SpaDES` module repositories
    
    b. Using [GitHub.com](https://github.com)
    
    c. `shiny` apps and [shinyapps.io](http://www.shinyapps.io/) (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))
    
    d. Data sources

8. Data to decisions

    a. Building a reproducible workflow

    b. Caching

## Resources:

- [SpaDES wiki](https://github.com/PredictiveEcology/SpaDES/wiki)
- [R documentation for `SpaDES`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0)
- [Development release of `SpaDES`](https://github.com/PredictiveEcology/SpaDES/tree/development)

