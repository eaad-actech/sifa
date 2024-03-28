# 4.5 Offsite Testing

This folder contains the production files for milling the cork blocks to reproduce the surveyed site. It also includes the survey of the milled surface and the comparision with the surveyed site.

## Surface milling
Surface milling was achieved in two steps. A roughing step to remove most material with a 3-axis strategy programed in Fusion360 and imported into Grasshopper for simulation and robot instruciton generation. A finishing step programed with Grasshopper.

## Comparison
The milled surfaces were surveyed using photogrametry. The photos were oriented and aligned using 3DF Zephyr. The dense point-cloud was filtered using reconstruction confidence and cropped to the area of interest. The resulting point-cloud was exported in E52 format. Later, the site survey and the modified site mesh were pre-aligned with the milled surface point cloud using Grasshopper. The Grasshopper file CP.gh allows pre-aligning and computing cloud-to-mesh distances to both pairs. 

For extra control, the pre-aligned meshes and the dense point-cloud were imported to CloudCompare to run ICP alignement and generate the images.