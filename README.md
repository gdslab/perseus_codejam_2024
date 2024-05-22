# 2024 Code Jam Repository

This is a repository for 2024 Code Jam. The goal of this code jam, hosted by the Institute for Digital Forestry at Purdue University, is to encourage innovation in a fun and active way. The winners will be announced at the 2024 PERSEUS Annual Meeting, Orono, Maine, July 22-24, 2024. Code jam participants will submit original codes and individual tree species identification results. The code jam organizers will evaluate the submitted codes and results on common data sets. 

The 2024 Code Jam will focus on **Auto-identification of tree species from 3D point cloud data**. We seek to automate the identification of tree species from 3D point cloud data. 

## Problem definition

Tree species identification is an essential part of sustainable forest management. New remote sensing technologies allow us to measure forests in greater detail. However, identifying tree species remains challenging. Creating better analytical tools to accomplish this goal will require creativity, innovation, and expertise from a wide range of skill areas. The 2024 Code Jam will challenge teams to develop novel methods for efficiently and accurately identifying tree species from high-resolution LiDAR point clouds.

## Input Data

We provide individual tree 3D point clouds and corresponding tree species labels in this competition. All data in this repository are collected in the Martell Forest using TLS (Terrestrial Laser Scanner). Individual tree segmentation was applied to the TLS 3D point cloud data using an Unsupervised Canopy-to-Root Pathing (UCRP) Tree Segmentation Algorithm (https://www.mdpi.com/2072-4292/14/17/4274) developed by Joshua Carpenter (a member of Geospatial Data Science Lab - https://gdsl.org). Tree species identification is based on the CFI (Continuous Forest Inventory) protocol and the most recent tree inventory campaign led by Dr. Songlin Fei's research group. 

### Individual tree 3D point cloud data

We provide individual tree 3D point cloud data in the **point_cloud** directory in the repository. Each file is assigned a numerical identifier, which will be used to match tree species labels. The file naming convention is **DDD.las**, where **DDD** represents the numerical identifier. 

### Tree species 

We provide tree species labels in the **spc.csv** file. This file has two columns: **tree_id** for the numerical identifier of the individual tree 3D point cloud data and **spc_code** for encoded tree species from **a** to **x** (A total of 26 species). We only provide encoded species labels for 368 trees. 

## What to submit

All participating teams need to submit the following to win a competition. 

* A brief report on the overall idea and process of the approach
* Programming source codes used to identify tree species
* A new **spc.csv** file that includes the encoded tree species for all 615 trees
