# MID360_Livox
Before cloning 
The following are the steps followed :

1) Install the LIVOX SDK : https://github.com/Livox-SDK/Livox-SDK2/blob/master/README.md
2) Clone this repository
3) Connect the Livox LAN and affix the IP of the ethernet
sudo ifconfig eth0 192.168.1.50 (replace “eth0” with the network port name of the computer)
4) Change the config and launch files
roscd livox_ros_driver2/config and change the host_net_info ips to 192.168.1.50 (the IP of your computer) and change the lidar_configs to the IP of the LIDAR

From the manual : "All Livox Mid-360 LiDAR sensors are set to static IP address mode by default with an IP address of 192.168.1.1XX (XX stands for the last two digits of the Livox Mid-360 LiDAR sensor’s serial number). The default subnet masks of the Livox Mid-360 LiDAR sensors are all 255.255.255.0 and their
default gateways are 192.168.1.1."

roscd livox_ros_driver2/launch and change rviz_MID_360.launch to reflect the change in the bd_list. (attached) The value can be found at the bottom of the LIVOX.

