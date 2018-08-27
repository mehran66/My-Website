+++
title = "Comparing the Accuracy of Interpolated Terrain Elevations Across Spatial Resolution"
date = 2018-07-01T00:00:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["**Mehran Ghandehari**", "Barbara P. Buttenfield", "Carson J. Q. Farmer"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["2"]

# Publication name and optional abbreviated version.
publication = "In *the International Journal of Remote Sensing (IJRS) (Under revision)*"
publication_short = ""

# Abstract and optional shortened version.
abstract = "Terrain is commonly modelled on a grid of pixels in Digital Elevation Model (DEM). Pixels are considered flat and rigid, for computational simplicity (a ‘rigid pixel’ paradigm). This paradigm does not account for the slope and curvature of terrain within each pixel, generating imprecise measurements, particularly as pixel size increases or in uneven terrain. Interpolation methods are commonly used to relaxe the rigid pixel assumption and reconstruct the surface of a pixel for estimating elevation, and terrain derivatives (e.g., slope and curvature) within a pixel (a ‘surface-adjusted’ paradigm). This paper aims to compare different interpolation methods to investigate possible sub-pixel variations for estimating elevation of arbitrary points given a regular grid. Tests based on interpolating elevation values for 20,000 georeferenced random points from a regular grid DEM are presented, using a variety of exact and inexact local deterministic interpolation methods within contiguity configurations incorporating first and second order neighbours. The paper examines the sensitivity of surface adjusted estimations across a progression of spatial resolutions (10 m, 30 m, 100 m, and 1000 m DEMs) and a suite of terrain types varying in latitude, altitude, slope, and roughness, validating sub-pixel variations against direct elevation measurements on 3 m resolution lidar data. Two mathematical surfaces with appropriately added noise are also used as artificial DEMs to have a data-independent methodology. Results illustrate that the Bi-cubic interpolation methods outperform Linear, and Bi-linear methods in most DEM resolutions and terrain types. However, when the vertical accuracy of DEM is decreased, Linear, and Bi-linear methods have the best performance. The type of contiguity configuration appears to play a role in estimation errors as well, with tighter neighbourhoods for most interpolation methods exhibiting higher accuracy. The analysis also considers the balance between the increased computations needed to measure surface-adjusted elevation against the improvement in accuracy."
abstract_short = ""

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's filename without extension.
#   E.g. `projects = ["deep-learning"]` references `content/project/deep-learning.md`.
#   Otherwise, set `projects = []`.
#projects = [""]

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = ""
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""


# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{name = "View Journal Article", url = "http://example.org"}]

# Does this page contain LaTeX math? (true/false)
math = false

# Does this page require source code highlighting? (true/false)
highlight = false

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = "headers/bubbles-wide.jpg"
caption = ""

+++

