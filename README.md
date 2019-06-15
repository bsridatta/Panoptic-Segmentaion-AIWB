# Panoptic Segmentation   
##### Internship @ AI Without Borders   


### Literature Study

|  Paper | bottom line | Constraints | Code | Dataset used |
| :--- | :--- | :--- | :--- | :--- |
|  [Panoptic Segmentation by FAIR](https://arxiv.org/pdf/1801.00868v3.pdf "Panoptic Segmentation by FAIR") | PQ - Considers segmentation quality and a recognition quality. PQ is insensitive to class imbalance by calculating for each class independently and average over classes. | Just an introduction to the task of panoptic segmentation | No code | Vistas, CityScapes, ADE20k |
|  [Panoptic Feature Pyramid Networks](https://arxiv.org/pdf/1901.02446.pdf "Panoptic Feature Pyramid Networks") | Detailed insights into the single-network architecture | Requires generating a coherent scene segmentation that is rich and complete. | No Code |  |
|  [UPSNet: A Unified Panoptic Segmentation Network<br/>](https://arxiv.org/pdf/1901.03784v2.pdf "UPSNet: A Unified Panoptic Segmentation Network<br/>") | 2 head network: Semantic Segmentation using Deformable Convolutions & Instance Segmentation using Mask R-CNN  | Complex and mutli-headed architecture, could be tricky to get it to work | [Uber Research](https://github.com/uber-research/UPSNet "Uber Research") | COCO, CityScapes |
|  Panoptic Segmentation with an End-to-End Cell R-CNN for Pathology Image Analysis | Panoptic segmentation of various cancer cells | Access to dataset. The paper does not mention details of the dataset nor if it was further modified to all pixel segmentation | No code | MICCAI 2017 digital pathology challenge dataset |


### Panoptic Datasets

|  Dataset | Classes | Evaluation Metrics |
| :--- | :--- | :--- |
|  [COCO 2018](http://cocodataset.org/index.htm#panoptic-2018 "COCO 2018") | Things, regions (Road, grass, water) | panoptic quality (PQ) |
|  [ADE20k](https://groups.csail.mit.edu/vision/datasets/ADE20K/ "ADE20k") | Things, regions and parts of things | Pixel Accuracy and IoU |
|  [Mapillary Vistas](https://www.mapillary.com/dataset/vistas "Mapillary Vistas") | Street Scenes | - |
|  [CityScapes](https://www.cityscapes-dataset.com/benchmarks/#panoptic-scene-labeling-task "CityScapes") | City/Street Scenes | PQ |
|  2017 MICCAI Digital Pathology Challenge dataset | Could not gain access - could be http://www.andrewjanowczyk.com/deep-learning/ or https://bioimage.ucsb.edu/research/bio-segmentation or  maybe should create one ourself for the task | - |

