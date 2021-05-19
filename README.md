# Home range analysis through Kernel Density Estimation in QGIS

The model created with the Graphical Model Builder in QGIS 3.16 allows to calculate the home range for a given level of density (typically 50% and 95%) through Kernel Density Estimation. Kernel Density is based on the Silverman's rule of Thumb. Please note that for a correct calculation of the home range, point locations must be in a projected reference system (i.e. UTM).

The model uses QGIS algorithms and works only for QGIS 3.16 (and later versions).

In order to use the model, download the model "Home Range KDE.model3" first, then open QGIS, go to the Processing options, and select Open an existing model... Navigate to the folder containing the model and DONE!
