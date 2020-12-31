# Thank you for downloading the plugin.

# Plugin for Qgis : DEMDrainageAnalyses

## Function : 
This plugin performs the following specific processing and analyzing tasks on drainage sites, using LiDAR data:

a. Extracts out all loaded checked vector and raster files within the boundary layer extent on the map canvas. Note: uncheck all web map layers from “QuickMapServives” like Google Satellite or Google Hybrid or OSM in the layers panel before pressing the OK button in the plugin.
b. Performs raster resampling to the desired pixel size desired. Note range of executable pixel size: 20 – 100 (ft).
c. Coverts the resampled raster layer to a vector point layer, by creating point features for each individual pixel's center in the raster layer.
d. Generates boundary lines into points layer and then join points to vector point layer
e. Exports the boundary lines points layer and the converted vector point layer to CSV files respectively, using the boundary layer extent. The CSV files can then be opened in excel. This function adds X and Y (or latitude/longitude) fields to the vector point layer.
f. All operations are saved in your specified subfolders accordingly. After all tasks have been executed and analyzed, go to the specified save folder and there you will see all 3 subfolders containing all files: “CSV_Files”, “Rasters”, and “Vectors”. The entire task of the plugin takes few seconds depending on the density of point
cloud data within the extent of the boundary layer extracted.

## Issues
You can report a issue [here](https://github.com/FVW-Services/DEM_drainage_analyses/issues/new) and check the current [issues](https://github.com/FVW-Services/DEM_drainage_analyses/issues).

## Developers :
Compile `ressources.py` with OSGeo4W Shell and the command : `pyrcc5 -o resources.py resources.qrc`

Edit `DEM_drainage_analyses_dialog_base.ui` with QT designer (in Qt Creator).

## Feedbacks
Feel free to contact us: fvw.services@gmail.com

## User Guide :
ILLINOIS DRAINAGE GUIDE (ONLINE) : http://www.wq.illinois.edu/DG/Extraction/LiDARThAn_Users_Guide.pdf