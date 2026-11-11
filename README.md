# Air-Gapped-Geospatial-ML-Inference-Platform-for-Multi-Sensor-Imagery

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/AbhigyanPandey08/Air-Gapped-Geospatial-ML-Inference-Platform-for-Multi-Sensor-Imagery/blob/main/notebooks/GeoVision_DIP_Complete_Portable_Superset.ipynb)

An academic Digital Image Processing project exploring portable image enhancement, feature representation, unsupervised clustering, and geospatial pattern analysis.

This portable image-processing framework that applies Digital Image Processing (DIP) techniques to ordinary digital images and multispectral geospatial imagery. It combines image enhancement, spatial filtering, spectral feature extraction, unsupervised clustering, and spatial pattern analysis in a reproducible Python workflow.

# Key Features:

Image loading, metadata inspection, and preprocessing

Contrast stretching, gamma correction, histogram equalization, and CLAHE

Gaussian smoothing, Sobel and Laplacian filtering, and Canny edge detection

NDVI and NDWI computation for compatible multispectral imagery

Feature standardization and MiniBatch K-Means clustering

Cluster visualization, silhouette analysis, and spectral summaries

Connected-component analysis and spatial patch characterization

Cluster-area estimation and georeferenced GeoTIFF export

Model saving, reloading, and prediction verification

# Study Area:

The initial geospatial application focuses on the BHU–Ganga River Corridor, Varanasi, India, using Sentinel-2 Level-2A imagery acquired on 26 December 2021.

The workflow is designed to be adaptable to other compatible image datasets and study areas.

# Technology Stack:

Python

Google Colab / Jupyter Notebook

NumPy, Pandas, Matplotlib

OpenCV, Pillow, scikit-image

Rasterio, GeoPandas

Scikit-learn

Repository Structure

GeoVision-DIP/
├── notebooks/
│   └── GeoVision_DIP_Complete_Portable_Superset.ipynb
├── data/
│   └── Input imagery (not included)
├── outputs/
│   └── Generated visualizations and raster products
├── docs/
│   └── Project documentation
└── README.md

# Getting Started:

Open the notebook in Google Colab or Jupyter Notebook.

Install the required dependencies.

Upload the input image or provide its local file path.

Configure the image bands where multispectral indices are required.

Execute the notebook sequentially to generate visualizations, clustering results, and output files.

# Methodology:

Input Imagery → Preprocessing → Image Enhancement → Spatial Filtering → Feature Extraction → Feature Standardization → Unsupervised Clustering → Spatial Analysis → Visualization and Export

# Novelty and Contribution:

The project integrates conventional DIP operations with unsupervised feature-based analysis in a common, portable workflow. Its key contribution is the comparative examination of how image enhancement and feature representation influence cluster separability and the spatial organization of image patterns.

# Limitations:

K-Means clusters represent spectral or feature-based groups, not verified semantic land-cover classes.

Silhouette scores measure cluster separation, not classification accuracy.

NDVI and NDWI require appropriate spectral bands; they are not meaningful for ordinary RGB images.

Area estimates require suitable geospatial metadata and a projected coordinate reference system.

The workflow is designed for local processing, but a genuinely air-gapped deployment requires locally available dependencies and input data.

# Reproducibility:

The notebook includes model serialization and reload verification to support repeatable processing. Results depend on the input imagery, preprocessing settings, feature configuration, and clustering parameters.

# Authors:

Pankaj Kumar & Abhigyan Pandey
B.Tech. Final Year Computer Science and Engineering
Rajiv Gandhi Institute of Petroleum Technology (RGIPT),
Bengaluru, India
