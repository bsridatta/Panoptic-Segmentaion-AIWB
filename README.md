# Panoptic Segmentation   
##### Internship @ AI Without Borders   


### Literature Study

|  Paper | Good To Know | Constraints | Code | Dataset used |
| :--- | :--- | :--- | :--- | :--- |
|  [Panoptic Segmentation by FAIR](https://arxiv.org/pdf/1801.00868v3.pdf "Panoptic Segmentation by FAIR") | PQ - Considers segmentation quality and a recognition quality. PQ is insensitive to class imbalance by calculating for each class independently and average over classes. | Requires generating a coherent scene segmentation that is rich and complete. Just an introduction to the task of panoptic segmentation | No code | Vistas, CityScapes, ADE20k |
|  [UPSNet: A Unified Panoptic Segmentation Network<br/>](https://arxiv.org/pdf/1901.03784v2.pdf "UPSNet: A Unified Panoptic Segmentation Network<br/>") | 2 head network: Semantic Segmentation using Deformable Convolutions & Instance Segmentation using Mask R-CNN  | Complex and mutli-headed architecture, could be tricky to get it to work | [Uber Research](https://github.com/uber-research/UPSNet "Uber Research") | COCO, CityScapes |


### Panoptic Datasets

|  Dataset | Entities | Evaluation |
| :--- | :--- | :--- |
|  [COCO 2018](http://cocodataset.org/index.htm#panoptic-2018 "COCO 2018") | Things, regions (Road, grass, water) | panoptic quality (PQ) |
|  [ADE20k](https://groups.csail.mit.edu/vision/datasets/ADE20K/ "ADE20k") | Things, regions and parts of things | Pixel Accuracy and IoU |
|  [Mapillary Vistas](https://www.mapillary.com/dataset/vistas "Mapillary Vistas") | Street Scenes |  |
|  [CityScapes](https://www.cityscapes-dataset.com/benchmarks/#panoptic-scene-labeling-task "CityScapes") | City/Street Scenes | PQ |
|  [Bio-Segmentation](https://bioimage.ucsb.edu/research/bio-segmentation "Bio-Segmentation") | Breast Cancer Cell, Liver etc<br/> | Custom Script |
