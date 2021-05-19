# Home range analysis through Kernel Density Estimation in QGIS

The model created with the Graphical Model Builder in QGIS 3.16 allows to calculate the home range for a given level of density (typically 50% and 95%) through Kernel Density Estimation. Kernel Density is based on the Silverman's rule of Thumb for search radius estimantion (unweighted distance).

![https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/GUID-3F1EEF03-5AFD-45BE-B001-6C960CD48534-web.png](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/GUID-3F1EEF03-5AFD-45BE-B001-6C960CD48534-web.png)

where:

- Dm is the median distance from mean center of the points.
- n is the number of points.
- SD is the standard distance.

The standard distance is computed as:

![https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/GUID-B7BB3366-2457-45A6-BEE5-EB230EC0B988-web.png](https://pro.arcgis.com/en/pro-app/latest/tool-reference/spatial-analyst/GUID-B7BB3366-2457-45A6-BEE5-EB230EC0B988-web.png)

where:
- x i , y i and z i are the coordinates for feature i
- {x̄, ȳ, z̄} represents the mean center for the features (if the coordinates z is present)
- n is equal to the total number of features.


Please note that for a correct calculation of the home range, point locations must be in a projected reference system (i.e. UTM).

The model uses QGIS algorithms and works only for QGIS 3.16 (and later versions).

In order to use the model, download the model "Home Range KDE.model3" first, then open QGIS, go to the Processing options, and select Open an existing model... Navigate to the folder containing the model and DONE!
