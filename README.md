# Panoptic Segmentation   
##### Internship @ AI Without Borders   

## Week - 1 
### Literature Study

|  Paper | bottom line | Constraints | Code | Dataset used |
| :--- | :--- | :--- | :--- | :--- |
|  [Panoptic Segmentation by FAIR](https://arxiv.org/pdf/1801.00868v3.pdf "Panoptic Segmentation by FAIR") | PQ - Considers segmentation quality and a recognition quality. PQ is insensitive to class imbalance by calculating for each class independently and average over classes. | Just an introduction to the task of panoptic segmentation | No code | Vistas, CityScapes, ADE20k |
|  [Panoptic Feature Pyramid Networks](https://arxiv.org/pdf/1901.02446.pdf "Panoptic Feature Pyramid Networks") | Detailed insights into the single-network architecture | Requires generating a coherent scene segmentation that is rich and complete. | No Code |  |
|  [UPSNet: A Unified Panoptic Segmentation Network](https://arxiv.org/pdf/1901.03784v2.pdf "UPSNet: A Unified Panoptic Segmentation Network<br/>") | 2 head network: Semantic Segmentation using Deformable Convolutions & Instance Segmentation using Mask R-CNN  | Complex and mutli-headed architecture, could be tricky to get it to work | [Uber Research](https://github.com/uber-research/UPSNet "Uber Research") | COCO, CityScapes |
|  [Panoptic Segmentation with an End-to-End Cell R-CNN for Pathology Image Analysis](https://link.springer.com/chapter/10.1007/978-3-030-00934-2_27) | Panoptic segmentation of various cancer cells | Access to dataset. The paper does not mention details of the dataset nor if it was further modified to all pixel segmentation | No code | MICCAI 2017 digital pathology challenge dataset |



## Week - 2
### Datasets

Specifically for Panoptic Segementation

|  Datasets | Description |
| :--- | :--- |
|  [COCO 2018](http://cocodataset.org/index.htm#panoptic-2018 "COCO 2018") | Things, regions (Road, grass, water) |
|  [ADE20k](https://groups.csail.mit.edu/vision/datasets/ADE20K/ "ADE20k") | Things, regions and parts of things |
|  [Mapillary Vistas](https://www.mapillary.com/dataset/vistas "Mapillary Vistas") | Street Scenes |
|  [CityScapes](https://www.cityscapes-dataset.com/benchmarks/#panoptic-scene-labeling-task "CityScapes") | City/Street Scenes |


Medical Image Datasets

|  Datasets | Description |
| :--- | :--- |
|  [2017 MICCAI Digital Pathology Challenge dataset](http://miccai.cloudapp.net/competitions/83 "2017 MICCAI Digital Pathology Challenge dataset") | Segmentation of Nuclei in Images. Dataset used in a paper for panoptic segmentation.<br/>Could not gain access to the dataset |
|  [Leukemia ALL-IDB](https://homes.di.unimi.it/scotti/all/ "Leukemia ALL-IDB") | (White) Blood cell classification. Looks suitable but have to download to know how the data is. |
|  [Multi-class artefact detection in video endoscopy](https://ead2019.grand-challenge.org/EAD2019/ "Multi-class artefact detection in video endoscopy") | Perfect dataset! But annotations are bounding box and not segementation. Have time to annotate? |
|  [ Blood Cells Detection](https://github.com/Shenggan/BCCD_Dataset " Blood Cells Detection") | Again perfect dataset! But annotations are bounding box and not segementation. Have time to annotate? |
|  [BACH](https://iciar2018-challenge.grand-challenge.org/Dataset/ "BACH") | Breast Cancer Histology Images. 1 huge whole slides with multiple classes and instances but cropped into 400 which mostly 1 instance and 1 class | 
|  [Melanoma, Skin Cancer](https://challenge2018.isic-archive.com/task1/training/ "Melanoma, Skin Cancer") | (Object segmentation)  Multi class segmentaion with 1 instance. |
|  [Segmentation of neuronal structures in EM stacks Home](http://brainiac2.mit.edu/isbi_challenge/ "Segmentation of neuronal structures in EM stacks Home") | Cell boundaries hence good for normal segmentation only |
|  [Nuclear Segmentation](https://www.dropbox.com/s/j3154xgkkpkri9w/IEEE_TMI_NuceliSegmentation.pdf?dl=0 "Nuclear Segmentation") | Good segmentation dataset but only nuclei, boundaries and background. Bascially 2 classes |
|  [Medical Segmentation Decathlon](https://decathlon-10.grand-challenge.org/ "Medical Segmentation Decathlon") | Huge number of datasets with no proper description |
|  [Broad Bioimage Benchmark Collection](https://data.broadinstitute.org/bbbc/image_sets.html "Broad Bioimage Benchmark Collection") | Database - with excellent description |
|  [The cell Image Library](http://cellimagelibrary.org/pages/datasets "The cell Image Library") | Database |
|  [ImageJ](https://imagej.net/Public_data_sets "ImageJ") | Database - Small |
|  [List of Cancer Cell Datasets for DL](http://www.andrewjanowczyk.com/deep-learning/ "List of Cancer Cell Datasets for DL") | Good datasets with multiclass classification but mostly for object detection (1 instance) |



## Week - 3
### Annotation tools and label format conversions
[Coco Annotator](https://github.com/jsbroks/coco-annotator/wiki)   
Quick annotaion of objects using 'Magic wand' to annotate disconnected objects or with the help of an API that fetches annotations from a semi-trained network. 

[voc2coco](https://github.com/yukkyo/voc2coco)  
Convert annotation format from voc to coco. Also contains direct instructions for the BCCD dataset [ Blood Cells Detection](https://github.com/Shenggan/BCCD_Dataset " Blood Cells Detection") mentioned above.

## Week - 4
### Downlaoding and reading annotation and trying the tools to make custom annotations
Setting up coco annotator docker. Downlaoding and coverting BCCD from VOC to coco. Takes quite some time to fully annotate each image. Very imbalanced instances. 
Reading artifact detection EAD dataset. Too many instances of blur and contrast which is immpossible to annotate for panoptic.
### Scraping the web one last time for a good dataset 
no luck

## Week - 5
### Going through the code 

