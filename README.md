# prisma-image-preprocessing
Python-based workflow implemented in Jupyter Notebook for geometric and radiometric correction of hyperspectral images from the PRISMA satellite.

### Geometric correction 

Geometric pre-processing uses the AROSICS co-registration algorithm (https://github.com/GFZ/arosics). A hyperspectral PRISMA image is used as the target image to be corrected, while a multispectral Landsat image with the same spatial resolution (30 m) is used as the reference image.

### Radiometric correction

Radiometric pre-processing includes the removal of water absorption bands and noisy spectral bands. Noisy bands are identified by comparison with reference spectra of grass measured in the field with an ASD FieldSpec® spectroradiometer.

This pre-processing workflow is designed to improve the geometric shift and spectral quality of PRISMA hyperspectral data for subsequent remote sensing analysis.

This repository was developed within the framework of the SEMHy-ARID project funded by the EO-Africa R&D Reseach facility and the European Space Agency (ESA).
