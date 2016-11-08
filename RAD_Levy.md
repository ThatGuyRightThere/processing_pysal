
#Austin Levy
##Spatial Smoothing - Pysal/QGIS
##GIS 441


1. Introduction
    1. Purpose of your package

    * Pysal-QGIS integration of a functional tool that allows the user to select between different spatial smoothing functions.

    2. Scope of your package

    * The scope of this package will be QGIS users.

    3. Objectives and success metrics for your project

1. Objectives

  * To successfully integrate a Pysal based smoothing package into QGIS to produce meaningful results.
With the integration data can be utilized by the variety of smoothing options.

2. Success metrics

Successful Integration as well as accuracy of results created by the smoothing.

 4. Definitions, terms

 * Mean Smoothing - a rate for each observation is replaced by an average of rates for its neighbors
 * Median Smoothing - the rate for an observation can be replaced by the median of the rates of its neighbors
 * Empirical Bayes Smoothing - adjust a raw rate by taking into account information in the other raw rates.
 * Non-parametric Smoothing -  compute rates without making any assumptions of distributional properties of rate estimates.


    5. References

https://pysal.readthedocs.io/en/v1.11.0/users/tutorials/smoothing.html

    6. Overview

This project will be focused around the benifits of the Pysal and QGIS integration. Pysal is a python based spatial tools library that QGIS does not poses for some areas.  Currently QGIS has no tool for spatial smoothing what so ever. By implementing a psyal based spatial smoothing toolkit it will allow users to analyze spatial rates without having to use third party software.

#### 2. Current System
###  1. Description of existing project you are enhancing

Pysal is an open source library of spatial tools and analytics written in the python language.

QGIS is also an open source piece of GIS software that we will be integrating Pysal into more and more as time goes on.



    2. How will you project extend existing work

Currently there is no spatial smoothing toolkit inside of QGIS but Pysal does have the packages to be able to make this a reality.


    3. What tasks does the new system support

The new tasks it will support are Mean and Median based Smoothing as well as Non-parametric smoothing and Empirical Bayes Smoothers.


#### 3. System Proposal
###  1. Overview

This toolkit will help to further the integration between the QGIS and Pysal libraries. With the Spatial Smoothing methods users will be able to realize the results in the QGIS GUI.

    2. Functional Requirements
        1. Listing of features to be implemented
          * Smoothing Toolkit
            * Mean Smoothing
            * Median Smoothing
            * Empirical Bayes Smoothing
            * Non-parametric Smoothing
          * As well as a GUI for the selection.
          * Python 2.7 will be used as QGIS does no support Python 3 yet.
          * Commented code that can easily be recreated
          * Users will only be able to select one method at a time
          * New output layer of the results will be displayed.


#### 3. Nonfunctional Requirements
        1. Useability

Usability will be a breeze. The user will be able to select a metric to use for the smoothing function from a drop down list such as homicide rates or disease metrics.

        2. Reliability

This package should always be reliable as there will most likely be very little changes if ever needed to keep it up to date.

        3. Performance

Performance should be pretty optimal as long as the data provided is correct and the data that the function is pulling is correct.

        4. Supportability

Supportability should also be incredibly easy. Even if the equations for calculating the spatial weights changes it's a simple change to make. This goes for the pysal packages needed as well.

        5. Implementation

Implementing this will be along the same lines as getting the processing pysal package into the toolbox.

        6. Interface

The GUI Interface will look very similar to all the other toolbox GUI’s for QGIS with drop downs for the selected catagories.

        7. Packaging
The packaging will the same as the processing pysal. Each form of smoothing will have its own file just like the morans as well as the pysal plug in and GUI needed to implement it.


        8. Licensing

This is using Pysal to be implemented in GQIS witch are both open source so no need to worry about licensing

#### 4. Project Management
    1. Schedule
        1. Detailed milestones for project


11/13/16
I would like to get the GUI knocked out first within the week as that is whats going to take the most time.

11/20/16
Implementing the smoothing paackages.

11/27 - 12/4
The last 2 weeks will be spent polishing and compatibility.

12/6
Presentation


    2. Repositories
        1. URL for project repository

https://github.com/ThatGuyRightThere/processing_pysal/test/project
