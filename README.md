# VideoObjectTracking
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->
[My LinkedIn](https://www.linkedin.com/in/vaidehi-lehekar/)



<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h3 align="center">Person Re-Identification using CCTV Footage</h3>

  <p align="center">
    
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#Data-Collection"> Step 1: Data Collection and Preprocessing </a></li>
        <li><a href="#Person-detection-and-tracking">Step 2:  Person Detection and Tracking </a></li>
        <li><a href="#Feature-Extraction"> Step 3: Feature Extraction </a></li>
        <li><a href="#Person-Re-identification-model">Step 4: Person Re-Identification Model </a></li>
        <li><a href="#Visualization-and-Demonstration">Step 5: Visualization and Demonstration </a></li>
        </li>
   
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

Objective: The objective of this assignment is to assess your computer vision skills in person reidentification using publicly available CCTV footage. You will develop a model to identify and
track individuals across multiple camera views.

<p align="right">(<a href="#readme-top">back to top</a>)</p>


### Testing Environment

Operating system:

1. MacOS Sonoma
   
Python package (Python 3.5 or Python3.6)
1. Tensorflow 1.8
2. Jupyter Notebook
4. opencv 3.3 (Need opencv dnn library)
5. Numpy
6. Ultralytics
7. yolov4



<!-- GETTING STARTED -->
## Getting Started
To start we first proceed with data collection as well as researching for the given problem statement
Installation of required libraries is performed as mentioned below

### Installation

```
!pip install ultralytics
```
```
!pip install roboflow>=0.2.31
```
<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Step 1: Data Collection and Preprocessing


The Video Footage has been obtained from the below source: 

[EPFL](https://www.epfl.ch/labs/cvlab/data/data-pom-index-php/):
On this page you can download a few multi-camera sequences that have been acquired by EPFL for developing and testing people detection and tracking framework. 
All videos, calibration and ground truth files available on this page are copyrighted by CVLab – EPFL. You can use them for research purposes. If you use them to publish
All of the sequences feature several synchronised video streams filming the same area under different angles. All cameras are located about 2 meters from the ground. All pedestrians on the sequences are members of people willingly participating in the research project.

The Camera Sequences selected are:
<img width="676" alt="Screenshot 2023-10-21 at 2 17 06 PM" src="https://github.com/Vaidehi5Lehekar/VideoObjectTracking/assets/62598069/bd8245fe-f368-43c1-96ce-317f89f43dcb">

<p align="center">Preprocessing </p>

<h4>Video to frame conversion</h4>
1. Create a folder with the input videos downloaded and a folder for the frames captured from the preprocessing.
2. Apply code for preprocessing. Refer the .ipynb file


### Step 2:  Person Detection and Tracking
Use Roboflow to perform preprocessing on the frames converted and then upload the dataset obtained for the yolo model from roboflow using the ultralytics model as shown in the code





