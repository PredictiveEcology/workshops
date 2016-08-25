# Introduction to ecological modelling with `SpaDES`

This workshop assumes good familiarity with R as well as several of its contributed packages.

## Topics covered

1. What is `SpaDES` and examples

    a. Fire – Beacons

    b. Vegetation simulation – SpaDES-Landis

    c. Agent models – [Wolves](http://htmlpreview.github.io/?https://github.com/PredictiveEcology/SpaDES-modules/blob/master/modules/wolfAlps/wolfAlps.html)

2. Building a new module from scratch

    a. create new module template: `newModule`

    b. the event queue

    c. initializing simulations: `simInit` and the `simList` object

    d. scheduling events: `scheduleEvent`

    e. running simulations: `spades`

    f. module metadata

    g. initializing data

    h. visualizing

3. Modules types


    a. events (*e.g.*, Fire)

    b. data modules (*e.g.*, climate data downloading)

    c. individual-based modules (*e.g.*, caribou)

4. Experiments and replication


    a. `experiment` function (replication, scenario creation, parameter experiments)

    b. running parallel simulations on supercomputers and clusters

    c. Pattern Oriented Modeling (`POM` function) for estimating unknown parameters

5. Power R for speed


    a. Spatial data (`raster` and `sp` packages)

    b. Matrices (for fast operations on numerics)

    c. `data.table` (for fast operations on `data.frames`, *i.e.*, columns of data)

6. Integrating across modules

    a. Building "models", *i.e.*, groups of modules

7. Online

    a. Using [GitHub.com](https://github.com)

    b. Using the `shiny` package for web interfaces (still in alpha state)

    c. Hosting `shiny` apps using [Shinyapps.io](http://www.shinyapps.io/) (*e.g.*, [Proof of concept](https://spades.shinyapps.io/ForestChange_ProofOfConcept/))

    d. Data sources

8. Data to decisions

    a. Building a reproducible workflow

    b. Caching

## Resources:

- [SpaDES wiki](https://github.com/PredictiveEcology/SpaDES/wiki)
- [R documentation for `SpaDES`](http://www.rdocumentation.org/packages/SpaDES/versions/1.2.0)
- [Development release of `SpaDES`](https://github.com/PredictiveEcology/SpaDES/tree/development)

