# Crop Monitoring System

This repository contains a Jupyter Notebook script for processing Sentinel-2 satellite images using Google Earth Engine (GEE). The script demonstrates various tasks such as filtering image collections, cloud masking, area normalization, and generating normalized difference vegetation index (NDVI) images to assess the health of crops in a specific area.

## Script Overview

The provided Jupyter Notebook script performs the following tasks:

1. **Setting Up Google Earth Engine:** Initializes GEE using a service account.
2. **Loading Sentinel-2 Image Collection:** Loads Sentinel-2 Surface Reflectance (SR) image collection.
3. **Filtering Images:** Filters images based on a specified date range and geometry.
4. **Cloud Probability Filtering:** Applies cloud masking using Sentinel-2 Cloud Probability image collection.
5. **Date Manipulation:** Calculates the interval between consecutive image dates.
6. **Equalizing Area of Interest:** Normalizes the area of interest across images.
7. **Adding NDVI Bands:** Calculates and adds the NDVI band to the image collection.
8. **Image Calculation:** Performs image calculations and generates the final composite image.
9. **Generating Normalized NDVI Image:** Generates a normalized NDVI image using area-normalized NDVI values.
10. **Exporting Results:** Exports the final image and vectorizes it for analysis.

## Output

The script generates a final area-normalized NDVI composite image. You can visualize, analyze, or export this image for further use.

## References

- [Google Earth Engine](https://earthengine.google.com/)
- [`geemap` Python Package](https://geemap.org/)
- [Sentinel-2 User Handbook](https://sentinel.esa.int/web/sentinel/user-guides/sentinel-2-msi)
