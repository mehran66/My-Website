+++
# Date this page was created.
date = 2018-04-27T00:00:00

# Project title.
title = "Surface Area Computations"

# Project summary to display on homepage.
summary = "Slope-Adjusted Surface Area Computations in Digital Terrain"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "sa.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["PhD"]

# Optional external URL for project (replaces project detail page).
external_link = "https://github.com/mehran66/Surface-Area-Computations"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "sa.jpg"
caption = "My caption :smile:"

+++

Area is an integral part of any spatial database and has a significant role in many geographic analyses and applications. Planar algorithms that are widely used to calculate area ignore the slope and curvature of the terrain and result in under-estimation, particularly as pixel size increases or in uneven terrain. Calculating surface area using a regular DEM can overcome this issue by considering localized variations on the terrain surface. This paper investigates the scale- and algorithm-dependence of surface area calculations. The expectation is that for any individual pixel, the improvement in measurements can be relatively small, however, the additive effects across the study area can become significant. The method of dividing each DEM pixel into eight 3D triangles is commonly used to calculate surface area. In this research, the elevation of triangle vertices are estimated using different interpolation methods to establish rates of under-estimation for progressively larger pixels. These methods are validated against vertex elevations on a 3 meter lidar data benchmark. Bi-Cubic interpolation outperforms other interpolation methods for calculating DEM surface areas, with Linear, Bi-Linear and Jenness methods performing nearly as well, especially at coarser resolution. 

Coding and statistical analysis are conducted in Python using open source modules (e.g., GDAL, Geopandas, numpy, scipy, and multiprocessing). The Amazon Web Services (AWS) is needed as a cloud computing service to handle large sets of DEM data, reduce time-to-results, and increases the speed of this research using high performance computers. In one of our study areas as an example, there are 25,500,000 pixels in the 10 m DEM. The surface area for each pixel should be calculated based on six different methods. This process is compute-intensive and very time-consuming, and the code needs to be parallelized to speed up the process. A virtual servers on AWS is used with 32 CPUs and 224 GB of RAM. This instance calculates surface area of 32 rows of DEM concurrently. Also, all of the computations are carried out in RAM and very large numpy arrays are saved in the memory.

Here is the strategy we consider to process larger data sets in AWS. A single DEM at a single resolution is partitioned into strips covering 5 rows and all columns to create a task pool. The justification for 5 rows is that the interpolation methods using 3rd order polynomials require 5*5 neighborhoods. Once uploaded, each strip is processed by one CPU to estimate surface area by all interpolation methods, storing the results in a numpy array. Therefore, the strips can be executed concurrently to calculate the surface area for the entire DEM. The calculate surface area raster for all methods and DEM resolutions are saved into disk and are subsequently downloaded for validation against the surface area calculate from the LiDAR benchmark. 

Referrence:	Mehran Ghandehari, and Barbara P. Buttenfield (2018). 'Slope-Adjusted Surface Area Computations in Digital Terrain', Proceedings of Geomorphometry 2018 conference, the 5th International Conference of the ISG, Boulder, Colorado, August 13-17