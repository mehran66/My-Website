+++
title = "Measuring Distance “As the Horse Runs”: Cross-Scale Comparison of Terrain-Based Metrics"
date = 2016-07-01T00:00:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Barbara P. Buttenfield", "**Mehran Ghandehari**", "Stefan Leyk", "Lawrence V. Stanislawski", "Meg Brantley", "Yi Qiang"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["1"]

# Publication name and optional abbreviated version.
publication = "In *The 9th International Conference on Geographic Information Science, GIScience 2016*"
publication_short = ""

# Abstract and optional shortened version.
abstract = "Distance metrics play significant roles in spatial modeling tasks, such as flood inundation (Tucker and Hancock 2010), stream extraction (Stanislawski et al. 2015), power line routing (Kiessling et al. 2003) and analysis of surface pollutants such as nitrogen (Harms et al. 2009). Avalanche risk is based on slope, aspect, and curvature, all directly computed from distance metrics (Gutiérrez 2012). Distance metrics anchor variogram analysis, kernel estimation, and spatial interpolation (Cressie 1993). Several approaches are employed to measure distance. Planar metrics measure straight line distance between two points (“as the crow flies”) and are simple and intuitive, but suffer from uncertainties. Planar metrics assume that Digital Elevation Model (DEM) pixels are rigid and flat, as tiny facets of ceramic tile approximating a continuous terrain surface. In truth, terrain can bend, twist and undulate within each pixel. Work with Light Detection and Ranging (lidar) data or High Resolution Topography to achieve precise measurements present challenges, as filtering can eliminate or distort significant features (Passalacqua et al. 2015). The current availability of lidar data is far from comprehensive in developed nations, and non-existent in many rural and undeveloped regions. Notwithstanding computational advances, distance estimation on DEMs has never been systematically assessed, due to assumptions that improvements are so small that surface adjustment is unwarranted. For individual pixels inaccuracies may be small, but additive effects can propagate dramatically, especially in regional models (e.g., disaster evacuation) or global models (e.g., sea level rise) where pixels span dozens to hundreds of kilometers (Usery et al 2003). Such models are increasingly common, lending compelling reasons to understand shortcomings in the use of planar distance metrics. Researchers have studied curvature-based terrain modeling. Jenny et al. (2011) use curvature to generate hierarchical terrain models. Schneider (2001) creates a ‘plausibility’ metric for DEM-extracted structure lines. d’Oleire-Oltmanns et al. (2014) adopt object-based image processing as an alternative to working with DEMs; acknowledging the pre-processing involved in converting terrain into an object model is computationally intensive, and  likely infeasible for some applications. This paper compares planar distance with surface adjusted distance, evolving from distance “as the crow flies” to distance “as the horse runs”. Several methods are compared for DEMs spanning a range of resolutions for the study area and validated against a 3 meter (m) lidar data benchmark. Error magnitudes vary with pixel size and with the method of surface adjustment. The rate of error increase may also vary with landscape type (terrain roughness, precipitation regimes and land settlement patterns). Cross-scale analysis for a single study area is reported here. Additional areas will be presented at the conference."
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
url_pdf = "Article/journal/GIScience16_Butenfield_etal.pdf"
url_preprint = ""
url_code = "https://github.com/mehran66/Surface-Adjusted-Distance"
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = "https://cloudfront.escholarship.org/dist/prd/content/qt8rh987cz/qt8rh987cz.pdf"

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
#image = "headers/IJRS2.jpg"
caption = ""


+++

