12345678901234567890123456789012345678901234567890123456789012345678901234567890
The files contained here represent the output from k-means clustering analysis 
of CVMS-4.26 using the built-in capabilities of MATLAB. Each analysis was run 
for a predefined value of K regions, ranging from 1 to 10. In order to mitigate 
some inherent biases from variations in velocity, we calculated the average 1D 
Vp an Vs profiles for S4.26 which are contained in the file, 
"Average_1D_S426.mat" and subtracted these averages from the full CVM before 
clustering. Additionally for the analysis of the concatenated Vs+Vp profiles 
(200 length vectors, termed "gamma" in the paper), we scaled the Vp portion by 
square root of 3 to avoid biasing the clusters with the greater Vp values. 

The output files are named based on data (VP, VS, or VSVP) and the K value 
(01-10). The remainder of the label indicates that these outputs were resorted 
so that the region numbers were consistent between K values (i.e., in K = 3, 1 is 
Continental Borderland, 2 is Batholith, 3 is Sedimentary Basins while K = 4, 1 is 
Continental Borderland, 2 is Batholiths, 3 is Sedimentary Basins, and 4 is 
Proterozoic Terranes as a new region). Each .mat file contains a variable 
"clusters" which contains the K centroid profiles for each corresponding region 
and "regions" which contains a numerical value for each node location in the model. 
The variable "regions" is a 1523712x1 matrix which can be reshaped to 992x1536 and 
produce pseudocolor images using MATLAB's pcolor function and defining a discrete 
colormap of K colors. 

If any more data is needed, please request by emailing me at eymold.1@osu.edu or 
beymold@gmail.com.

Billy Eymold October 15, 2019
