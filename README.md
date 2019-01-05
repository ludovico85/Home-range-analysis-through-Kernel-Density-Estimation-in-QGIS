# Home range analysis through Kernel Density Estimation in QGIS

The model created with the Graphical Model Builder in QGIS 3.4 allows to calculate the home range for a given level of density (tipycally 50% and 95%) through Kernel Density Estimation. Kernel Density is based on the Silverman's rule of Thumb. Please note that for a correct calculation of the home range, point locations must be in a projceted reference system (i.e. UTM).

<img src = "https://www.lezionigis.it/wp-content/uploads/2019/01/KDE8-1024x388.png"></img>

The model uses QGIS algorithms and works only for QGIS 3.4 (Madeira).

In order to use the model, download the model "Home Range KDE.model3" first, then open QGIS, go to the Processing options, and select Open an existing model... Navigate to the folder containing the model and DONE!

<img src = "https://www.lezionigis.it/wp-content/uploads/2019/01/Processing.png"></img>



A detailed description of the algorithm used is available at https://www.lezionigis.it/tutorial-n-6-calcolo-dellhome-range-kernel-density-estimation/ (in italian only).