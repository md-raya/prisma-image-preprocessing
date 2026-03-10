# prisma-image-preprocessing
--
Python-based workflow implemented in Jupyter Notebook for geometric and radiometric correction of hyperspectral images from the PRISMA satellite.

This repository was developed within the framework of the SEMHy-ARID project funded by the [EO-Africa R&D Reseach facility](https://www.eoafrica-rd.org/) and the [European Space Agency (ESA)](https://www.esa.int/).

This pre-processing workflow is designed to improve the geometric shift and spectral quality of PRISMA hyperspectral data for subsequent remote sensing analysis.

- **Geometric correction** 

Geometric pre-processing uses the AROSICS co-registration algorithm (https://github.com/GFZ/arosics). A hyperspectral PRISMA image is used as the target image to be corrected, while a multispectral Landsat image with the same spatial resolution (30 m) is used as the reference image.

- **Radiometric correction**

Radiometric pre-processing includes the removal of water absorption bands and noisy spectral bands. Noisy bands are identified by comparison with reference spectra of grass measured in the field with an ASD FieldSpec® spectroradiometer.

# Instalation
--
The following libraries will be needed to properly use the Jupyter Notebook:
- gdal
- geopandas
- cartopy
- joblib >=1.3.0
- matplotlib
- numpy
- pandas
- pyproj >2.2.0
- scikit-image >=0.21.0
- shapely
- rasterio
- notebook

# Contributors
--
María Dolores Raya-Sereno
Vicente Burchard-Levine

# License
--
prisma-image-preprocessing

Copyright 2026 María Dolores Raya-Sereno and contributors.

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program. If not, see http://www.gnu.org/licenses/.
