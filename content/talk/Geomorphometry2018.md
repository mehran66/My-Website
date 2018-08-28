+++
title = "'Slope-Adjusted Surface Area Computations in Digital Terrain"
date = 2018-08-01T00:00:00  # Schedule page publish date.
draft = false

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
time_start = 2018-08-13T13:00:00
time_end = 2018-08-17T15:00:00

# Abstract and optional shortened version.
abstract = "Area is an integral part of any spatial database and has a significant role in many geographic analyses and applications. Planar algorithms that are widely used to calculate area ignore the slope and curvature of the terrain and result in under-estimation, particularly as pixel size increases or in uneven terrain. Calculating surface area using a regular DEM can overcome this issue by considering localized variations on the terrain surface. This paper investigates the scale- and algorithm-dependence of surface area calculations. The expectation is that for any individual pixel, the improvement in measurements can be relatively small, however, the additive effects across the study area can become significant. The method of dividing each DEM pixel into eight 3D triangles is commonly used to calculate surface area. In this research, the elevation of triangle vertices are estimated using different interpolation methods to establish rates of under-estimation for progressively larger pixels. These methods are validated against vertex elevations on a 3 meter lidar data benchmark. Bi-Cubic interpolation outperforms other interpolation methods for calculating DEM surface areas, with Linear, Bi-Linear and Jenness methods performing nearly as well, especially at coarser resolution. Relative accuracies are shown to degrade somewhat in rougher terrain."
abstract_short = ""

# Name of event and optional event URL.
event = "Geomorphometry 2018 conference, the 5th International Conference of the ISG"
event_url = "http://2018.geomorphometry.org/"

# Location of event.
location = "Boulder, Colorado"

# Is this a selected talk? (true/false)
selected = false

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter your project's filename without extension.
#   E.g. `projects = ["deep-learning"]` references `content/project/deep-learning.md`.
#   Otherwise, set `projects = []`.
#projects = ["deep-learning"]

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = "Article/Conference/Ghandehari_Geomorphometry18_Published.pdf"
url_slides = "Article/Conference/Ghandehari_Geomorphometry18_powpoint.pdf"
url_video = ""
url_code = "https://github.com/mehran66/Surface-Area-Computations"

# Does the content use math formatting?
math = true

# Does the content use source code highlighting?
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
#image = "headers/bubbles-wide.jpg"
caption = ""

+++

Mehran Ghandehari, and Barbara P. Buttenfield (2018). 'Slope-Adjusted Surface Area Computations in Digital Terrain', Proceedings of Geomorphometry 2018 conference, the 5th International Conference of the ISG, Boulder, Colorado, August 13-17