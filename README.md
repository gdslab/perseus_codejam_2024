# 2024 Code Jam Repository

<img src="https://github.com/gdslab/perseus_codejam_2024/blob/main/figures/digital-forest-projects.jpg" width="100%">

This is a repository for 2024 Code Jam. The goal of this code jam, hosted by the Institute for Digital Forestry at Purdue University, is to encourage innovation in a fun and active way. The winners will be announced at the 2024 PERSEUS Annual Meeting, Orono, Maine, July 22-24, 2024. Code jam participants will submit original codes and individual tree species identification results. The code jam organizers will evaluate the submitted codes and results on common data sets. 

The 2024 Code Jam will focus on **Auto-identification of tree species from 3D point cloud data**. We seek to automate tree species identification from 3D point cloud data. 

## Problem definition

Tree species is a fundamental information required for forest inventorying, yet it has been a challenging task through remote sensing data. Many methods have been developed but lack generalizability. Here, we invite all PERSUS collaborators to bring your knowledge and expertise to unravel the novel method to identify tree species based on LiDAR data. This competition is divided into two sections: a. description of methods submission, and b. classification results. We are counting on you!

## Input Data

LiDAR data was collected within the central hardwood forests during the leaf-off season. The raw data was collected using a FARO laser scanner set about 1.5 meters above the ground. Only one scan was collected at each location, so the point cloud data contains many exclusions. Individual trees were split out of the raw point cloud using a tree segmentation algorithm. Each .las file provided is intended to represent only one tree. Some noise and a few segmentation errors may be present in the provided data.  

We provide individual tree 3D point clouds and corresponding tree species labels in this competition. All data in this repository are collected in the Martell Forest using TLS (Terrestrial Laser Scanner). Individual tree segmentation was applied to the TLS 3D point cloud data using an Unsupervised Canopy-to-Root Pathing (UCRP) Tree Segmentation Algorithm (https://www.mdpi.com/2072-4292/14/17/4274) developed by Joshua Carpenter (a member of Geospatial Data Science Lab - https://gdsl.org). Tree species identification is based on the CFI (Continuous Forest Inventory) protocol and the most recent tree inventory campaign led by Dr. Songlin Fei's research group. 

### Individual tree 3D point cloud data

<img src="https://github.com/gdslab/perseus_codejam_2024/blob/main/figures/codejam_ex.png" width="600 px">

We provide individual tree 3D point cloud data in the **point_cloud** directory in the repository. Each file is assigned a numerical identifier, which will be used to match tree species labels. The file naming convention is **DDD.las**, where **DDD** represents the numerical identifier. 

### Tree species 

We provide tree species labels in the **spc.csv** file. This file has two columns: **tree_id** for the numerical identifier of the individual tree 3D point cloud data and **spc_code** for tree species. We used an alphabet encoder for the tree species. The encoded value ranges from **a** to **x**, which contains 24 species in total. We provide encoded species labels for 368 trees to train your own model. 

## What to submit

All participating teams need to submit the following to win a competition. 

* A brief report on the overall idea and process of the approach
* Programming source codes used to identify tree species
* A new **spc.csv** file that includes the encoded tree species for all 616 trees

## Where to submit

You need to submit the abovementioned items to Bina Thapa (thapab@purdue.edu). 

# License

All data in this repository can only used for the 2024 Code Jam, and they **CANNOT** be used for anything else. If you want to use this data for publications, please contact Dr. Jinha Jung (jinha@purdue.edu) and Dr. Songlin Fei (sfei@purdue.edu) to get an appropriate agreement. 

# Acknoweldgement

Some text will come here.


