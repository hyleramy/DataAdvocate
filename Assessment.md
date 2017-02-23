---
layout: default
title: Assessment
---
# Project Assessment

Assessing the variability and characteristics of the Square Lake area requires the use of multiple applications. In this study, LAStools, SAGA-GIS, and ArcGIS were utilized throughout this assessment to evaluate the characteristics of this area.

## ESRI Software


<a href="http://tinypic.com?ref=4lspw0" target="_blank"><img src="http://i67.tinypic.com/4lspw0.jpg" border="0" alt="Image and video hosting by TinyPic"></a> <a href="http://tinypic.com?ref=md145u" target="_blank"><img src="http://i67.tinypic.com/md145u.jpg" border="0" alt="Image and video hosting by TinyPic"></a> <a href="http://tinypic.com?ref=21ay2yo" target="_blank"><img src="http://i65.tinypic.com/21ay2yo.jpg" border="0" alt="Image and video hosting by TinyPic"></a> <a href="http://tinypic.com?ref=acppar" target="_blank"><img src="http://i63.tinypic.com/acppar.jpg" border="0" alt="Image and video hosting by TinyPic"></a>

## LAStools

### Interface

LAStools ground classification program allows the point cloud downloaded from NOAA to be reclassified to select only the ground points within this subject area. This is a tool for bare-earth extraction: it classifies LIDAR points into ground points (class = 2) and non-ground points (class = 1). This is a totally redesigned version of lasground that handles complicated terrain much better where there are steep mountains nearby urban areas with many buildings. For the purpose of this analysis, I used the '-nature' option that uses a step size of 5 meters for terrains without buildings. But doing this, we are able to get the ground returns where accessible.

<a href="http://tinypic.com?ref=wlq8t5" target="_blank"><img src="http://i68.tinypic.com/wlq8t5.jpg" border="0" alt="Image and video hosting by TinyPic"></a>

### Ground Point Elevation


<a href="http://tinypic.com?ref=34gn1ud" target="_blank"><img src="http://i64.tinypic.com/34gn1ud.jpg" border="0" alt="Image and video hosting by TinyPic"></a>


### Ground Point Classification

lasground.exe extracts the bare-earth by classifying all ground points.This image shows the ground points classified within the area. As you can see, the majority of ground points have been extracted providing evidence that this area is "ground" rather than hydrology.

<a href="http://tinypic.com?ref=eas6md" target="_blank"><img src="http://i64.tinypic.com/eas6md.jpg" border="0" alt="Image and video hosting by TinyPic"></a>

When we zoom into the extracted point cloud, you'll notice the differences in elevation as well as building footprints in white. This further supports the distiction between ground and hydrology.

<a href="http://tinypic.com?ref=t6p9tw" target="_blank"><img src="http://i66.tinypic.com/t6p9tw.jpg" border="0" alt="Image and video hosting by TinyPic"></a>










<body class="theme-base-0d"></body>
