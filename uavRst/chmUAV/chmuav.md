Creating a UAV based Digital Surface Model from RGB imagery derived point clouds
================

Digital Surface Models
----------------------

Digital Surface Models (DSMs) are very useful and common data sets in numerous spatial and environmental problems such as ecological, hydrological or meteorological and so on. High resolution DSM/DTM are nowadays usually derived from LiDAR data. However this is expensive and not always and everywhere available. Lowest Budget ready to fly unmanned vehicles (rtf-UAVs) are very suitable to close this gap for a fast and reasonable retrieval of imagery data and and as a derivative of it dense point clouds (DPCs).

Prerequisites
-------------

To derive Orthoimages or point clouds one can use between different tools the tutorial data is produced using [Agisoft Photoscan](http://www.agisoft.com) which is a great tool for deriving point clouds and all kind of surface models. In the end of the processing chain you will have an orthorectified image and a dense point cloud. We will use some UAV data from the Marburg Open Forest project.

First attempt
-------------

First we have to set up the project. This is obviously more than usually due to the fact that a bunch of software needs to be linked against R. f

    ## Loading required package: uavRst

    ## Loading required package: raster

    ## Loading required package: sp

    ## Loading required package: mapview

    ## 1

    ## :: calculate DSM...
    ## :: convert raw DSM to GeoTiff 
    ## :: fill no data... 
    ## :: smoothing the gap filled DSM... 
    ## :: calculate metadata ...

![](chmuav_files/figure-markdown_github/dsm1-1.png) \#\# Second attempt

we want to have a coarser and smoother result, so we can change the filter and resolution options.

    ## :: calculate DSM...
    ## :: convert raw DSM to GeoTiff 
    ## :: fill no data... 
    ## :: smoothing the gap filled DSM... 
    ## :: calculate metadata ...

![](chmuav_files/figure-markdown_github/dsm2%20-1.png)
