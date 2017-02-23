---
layout: default
title: Assessment
---
# Project Assessment

Assessing the variability and characteristics of the Square Lake area requires the use of multiple applications. In this study, LAStools, SAGA-GIS, and ArcGIS were utilized throughout this assessment to evaluate the characteristics of this area.

## ESRI Software

### ArcMap

The following images are created through ESRI's ArcMap program. The point cloud .las file downloaded from NOAA was imported into a .las database created using ArcCatalog. When adding this file to the geodatabase, statistics are automatically calculated for this raw data and configured to the specs provided. 
* Image (A) is raw point file for the site of interest identified in red
* Image (B) is the aerial image use as a land classification cross reference
* Image (C) is the hillshade created from the .las file DEM
* Image (D) is the DEM created overlaying the hillshade for better visualization

<p align="center"> 
 <a href="http://tinypic.com?ref=1673sjl" target="_blank"><img src="http://i65.tinypic.com/1673sjl.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
</p>

As you can see by this visualization, the elevation is noticably lower in the green areas and higher in the red. For this site in Florida, the surface is very low and flat making it difficult to determine ground or hydrology through visualization. Further analysis must be assessed to evaluate the area and extract bare-earth points to classify ground versus hydrology.

## LAStools

### Interface

LAStools ground classification program allows the point cloud downloaded from NOAA to be reclassified to select only the ground points within this subject area. This is a tool for bare-earth extraction: it classifies LIDAR points into ground points (class = 2) and non-ground points (class = 1). This is a totally redesigned version of lasground that handles complicated terrain much better where there are steep mountains nearby urban areas with many buildings. For the purpose of this analysis, I used the '-nature' option that uses a step size of 5 meters for terrains without buildings. But doing this, we are able to get the ground returns where accessible.

<p align="center"> 
  <a href="http://tinypic.com?ref=wlq8t5" target="_blank"><img src="http://i68.tinypic.com/wlq8t5.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
</p>

### Ground Point Elevation

<p align="center"> 
  <a href="http://tinypic.com?ref=34gn1ud" target="_blank"><img src="http://i64.tinypic.com/34gn1ud.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
</p>

### Ground Point Classification

lasground.exe extracts the bare-earth by classifying all ground points.This image shows the ground points classified within the area. As you can see, the majority of ground points have been extracted providing evidence that this area is "ground" rather than hydrology.

<p align="center"> 
  <a href="http://tinypic.com?ref=eas6md" target="_blank"><img src="http://i64.tinypic.com/eas6md.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
</p>

When we zoom into the extracted point cloud, you'll notice the differences in elevation as well as building footprints in white. This further supports the distiction between ground and hydrology.

<p align="center"> 
  <a href="http://tinypic.com?ref=t6p9tw" target="_blank"><img src="http://i66.tinypic.com/t6p9tw.jpg" border="0" alt="Image and video hosting by TinyPic"></a>
</p>

Although this method successfully extracts ground points from the .las data set, further evaluation must be execuated to ensure the consistency of spatial data. The sections surrounding this "Square Lake" should also be looked at to determine whether the surrounding area is consistent with these findings. Since this is a good foundation toward understanding the geography of the area, the data obtain imposes challenges with the NOAA data classification (e.g. two classifications: ground & road).









<body class="theme-base-0d"></body>
