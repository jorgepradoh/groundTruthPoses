# groundTruthPoses

With this livescript we can extract the ground truth matrix required as a '.mat' format
in MATLAB for Visual Odometry and SLAM

In the example we extract the ground truth data by performing the necesary rotation and translation 
operations to get the viewId, Location, and Orientation cell for each instance in the ground truth data.

The script expects a '.csv' file containing GNSS 5DoF gound truth as the following data in this specific order: 

% UNIX time, GPSweek, GPST(s), x-enu(m), y-enu(m), z-enu(m), std-e(m), std-n(m), std-u(m), orientation.w, orientation.x, orientation.y, orientation.z, std-eulerx(rad), std-eulery(rad), std-eulerz(rad), v-e(m/s), v-n(m/s), v-u(m/s), std-ve(m/s), std-vn(m/s), std-vu(m/s) 

For our example we use one MADMAX Planetary Dataset's (cited at the end of the README) trajectory, but it will work with any data that meets the previously specified requirements.



Meyer, L., Smíšek, M., Fontan Villacampa, A., Oliva Maza, L., Medina, D., Schuster, M. J., Steidle, F., Vayugundla, M., Müller, M. G., Rebele, B., Wedler, A., & Triebel, R. (2021). The MADMAX data set for visual‐inertial rover navigation on Mars. Journal of Field Robotics, 1– 21. https://doi.org/10.1002/rob.22016
