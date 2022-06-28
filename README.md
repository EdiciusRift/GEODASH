## User Manual of GEODASH - Geotagging and Object Detection using Dashcam
#### I. Introduction
GEODASH is a system that can be used to detect traffic signs, and geotag the detected traffic signs and pin them on a map. The geotagged traffic signs can be used as an early warning device by the users who are not familiar with the area. This user manual will guide the user on how to operate GEODASH properly.
#### II. Requirements
GEODASH does not need to be operated on a high-end machine since it is uploaded to Google Colaboratory. Any machine that is capable of uploading and downloading data on a browser is enough to operate GEODASH. However, these are the additional requirements that are needed by the system for it to properly operate:
##### A. Dashboard camera footage (Preferably with a maximum duration of 2 minutes);
##### B. Corresponding GPS data of the footage; and
##### C. Corresponding Magnetometer data of the footage
There is no strict format to the file names of the requirements since the corresponding file names will be manually inputted to the system by the user.
##### NOTE: If there is at least one requirement that is not present, the system will fail to operate.
#### III. How to Operate GEODASH
##### A. Uploading of the requirements
The dashboard camera footage, corresponding GPS data of the footage, and corresponding Magnetometer data of the footage can be uploaded to either Google Drive or directly to the Google Colaboratory notebook where GEODASH is uploaded.
##### B. Linking the uploaded requirements to the notebook
The user should manually input the corresponding file names of the footage, GPS data, and Magnetometer data to cell #5 (see Figure 1 for reference) of the notebook to link the corresponding files to the notebook

![Figure 1](../main/Figure_1.png)
###### Figure 1: Cell #5 of the notebook where video_file_name, GPS_file_name, and  Magnetometer_file_name correspond to the file names of the footage, GPS file, and Magnetometer file, respectively.
##### C. Running the system
Under the *Runtime* tab of the Google Colaboratory Menu bar, a *Run all* command (see Figure 2 for reference) can be clicked by the user to operate the system. Alternatively, the user can press *Ctrl + F9* as a shortcut to operate the system. The system should automatically read all of the requirements, place the detected traffic signs inside the database, and show the geotagged locations of the detected traffic signs on Google Maps.

![Figure 2](../main/Figure_2.png)
###### Figure 2: Run all command under the Runtime tab of the Google Colaboratory Menu bar. Alternatively, Ctrl + F9 can be used as a shortcut to do the same command.
