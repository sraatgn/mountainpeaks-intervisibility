[TOC]

# Hiking in Appennino Tosco-Emiliano: Elevation & Intervisibility Analysis

This repository contains the code and data used to analyze the area surrounding Appennino Tosco-Emiliano National Park, focusing on elevation and intervisibility of mountain peaks and hiking trails within this region.

## Replicate results
The analysis can be replicated by:
1. Cloning this repository in the desired directory
``` 
git clone https://github.com/sraatgn/mountainpeaks-intervisibility.git
```
2. In that directory (`cd <dir/path>`), create a virtual environment:
``` 
python -m venv <envname>
```
3. Activate environment:
```
# On Windows
<envname>\Scripts\activate
# On macOS/Linux
source <envname>/bin/activate
```
4. Install required packages:
```
pip install -r requirements.txt
```
Large files (DEM and QGIS result layers) are not included, but can be retrieved by following the analysis workflow. 
The other data (geoJSON files) for Appennino Tosco-Emiliano is already available in the `data/` and `qgis_layers` directory. 
It is possible to analyze a different area by adjusting the bounding box used (`bbox_geom`) to download data for a different region.

## Contents
- `data/`: downloaded datasets.
- `qgis_analysis/`
    - `qgis_layers`: loaded layers for intervisibility analysis. 
	- `commands.txt`: commands to replicate analysis.
	- `visibility_analysis.qgz`: QGIS project.
- `dem_and_peaks.ipynb`: notebook used for DEM and mountain peaks download, preprocessing and analysis.
- `trail_analysis.ipynb`: notebook used for hiking trails and viewpoints download, preprocessing and analysis.

## Example Results
![An example of the result: network of visible peaks from Pietra di Bismantova](repoimg.png)

## Authors
- Sara Tegoni [@sraatgn](https://github.com/sraatgn)