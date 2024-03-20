# STSD
A large-scale, multi-modal dataset for semantic segmentation of subway tunnel point cloud called subway tunnel segmentation dataset (STSD) is proposed. The STSD comprises point clouds and projected images annotated into 11 categories, encompassing three types of subway tunnels with a combined length exceeding 2700 meters, totaling over 2.26 billion points.

## Download

Please fill this [**Data request form**](https://docs.google.com/forms/d/1TJChwoanKUs9qZhckt_v5rv9QElYH0Dfx-_aD5ofsEQ/edit)

Download links will be sent automatically after completing the application.

## Dataset
### 1.1 Overview
STSD is a multi-modal dataset for semantic segmentation of subway tunnels point cloud, consisting of two modality, point cloud and projected images. Three types of subway tunnels, quasi-rectangular, horseshoe, and circular is included in STSD.
<img src="img\fig2.png" alt="Network" style="zoom:100%;" />
Fig.1. Examples of subway tunnels point clouds. (a) Quasi-rectangular tunnel, (b)horseshoe-shaped tunnel, (c) circular tunnel.

A typical segment of tunnel data in STSD is as follows:
<img src="img\fig5.png" alt="Network" style="zoom:100%;" />
Fig.2. Example of a quasi-rectangular tunnel segment in STSD dataset: (a) side view of point cloud colored by intensity, (b) side view of point cloud colored by category, (c) top view of point cloud, (d) label visualization image, (e) label channel image, (f) H channel image, (g) Z channel image, (h) intensity channel image. 

Table 1. Details of the data source
<img src="img\fig3.png" alt="Network" style="zoom:40%;" />

<img src="img\fig9.png" alt="Network" style="zoom:40%;" />    

Fig.3.Overall top view of subway tunnel point cloud used in STSD (The discontinuous parts in the point cloud of the quasi-rectangular and circular tunnels are subway stations, their point cloud was excluded from the data source).      


The tunnel is divided into 264 segments, with each segment consisting of annotated LAS files of point clouds, along with annotated image files. The details of image are as follows:  
<img src="img\fig4.png" alt="Network" style="zoom:40%;" />

### 1.2 Data collection
The data was collected with Rail Mobile Measurement System (rMMS), which was introducted in our previous work [**Shield subway tunnel deformation detection based on mobile laser scanning**](https://www.sciencedirect.com/science/article/pii/S0926580518309737) 

### 1.3 Annotation Detail
Table 2. Annotation details of subway tunnels in STSD
<img src="img\fig1.png" alt="Network" style="zoom:40%;" />

<img src="img\fig10.png" alt="Network" style="zoom:100%;" />
Fig.4.(a) Color legend, (b-d) Labeled projected image of Quasi-rectangular tunnel, horseshoe-shaped tunnel, circular tunnel.


### 1.4 Label distribution of STSD
<img src="img\fig6.png" alt="Network" style="zoom:100%;" />
Fig.5. Statistics of STSD.

### 1.5 Benchmark
STSD is tested in several DL 2D and 3D segmentation networks, including classical and state-of-the-art ones, to verify its availability.

Table 3. Evaluation IoU results of each model on STSD. (The best result for each row is bolded. First five segmentation models use 2D IZH channel input, and the last two segmentation models use 3D XYZI input)
<img src="img\fig7.png" alt="Network" style="zoom:100%;" />

<img src="img\fig8.png" alt="Network" style="zoom:100%;" />
Fig.6. Detailed comparison of point cloud semantic segmentation results of each model: (a) Intensity, (b) Ground truth, (c) HRNet, (d) OCRNet, (e) DeepLabv3+, (f) PSPNet, (g) SegFormer, (h) RandLA-Net, (i) SCF-Net.


