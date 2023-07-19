---
layout: page
title: ""
---
This MATLAB package extracts MCSs from gridded IR images of a geostationary satellite. The tracking is based on the overlap technique (Williams and Houze, 1987) where the continuity of an MCS is decided according to the overlaps in two frames.

1. Use Grid_data.m for gridding raw data from satellite.
2. Run Track_CS.m for tracking of MCSs in the gridded dataset.
3. MCS are stored in .csv files in the 'MCSs_dataset' folder.

Note: The LAT-LON grid can be set to (1/12) degree spatial resolution. The native Kalpna-1 image resolution is 8 km. The native INSAT-3D/INSAT-3DR image resolution is 4 km. Modify the spatial resolution of the grid as needed.

Tracking dataset columns:

ID, Day, Month, Hour, Minutes, lat, lon, Area, ImageNumber, SplitParentID, MergeParentID, MergeChldArea, MinTemperature, CoreArea, AvgTemperature

<p align="center">
<img src="/assets/Tracking.gif" width="850" height="500">	
</p>

Code is available on my Github repository: <br> 
<a href="https://github.com/jayphd/Track_MCSs/"> https://github.com/jayphd/Track_MCSs/ </a>

References: <br>

Phadtare, J. and Bhat, G.S., 2019. Characteristics of deep cloud systems under weak and strong synoptic forcing during the Indian summer monsoon season. Monthly Weather Review, 147(10), pp.3741-3758. DOI: https://doi.org/10.1175/MWR-D-18-0346.1 <br>

Williams, M., and R. A. Houze, 1987: Satellite-observed characteristics of winter monsoon cloud clusters. Mon. Wea. Rev., 115 (2), 505–519. <br>

Contact: Jayesh Phadtare. jayesh.phadtare@gmail.com
