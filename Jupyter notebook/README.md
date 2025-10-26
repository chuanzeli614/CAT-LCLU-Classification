# Notebooks: Training, Prediction & Mosaicking

This folder contains two Jupyter notebooks that cover the land-cover classification workflow in the Cerrado–Amazon Transition (CAT) region.

Contents:

'Unet_Train_Validation.ipynb`
  - A U-Net for 2D segmentation with TensorFlow/Keras.

`raster_tiling_predict_mosaic.ipynb`
  - Tiling: slides a window across a large raster.
  - Prediction: loads the trained model, predicts per-pixel classes, and writes rasters.
  - Remove overlapping border for tile.
  - Merge: mosaics predicted tiles back into a single GeoTIFF.

Environment:

- Python 3.9+
- TensorFlow 2.10+ (GPU recommended), Keras
- `rasterio`, `GDAL`/`osgeo`, `numpy`, `scikit-learn`
