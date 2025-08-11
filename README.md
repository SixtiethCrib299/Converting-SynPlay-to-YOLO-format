SynPlay (https://arxiv.org/abs/2408.11814) is a synthetic dataset in the UAV domain. It contains human 2D/3D bounding boxes (BBXs), segmentation, and more, all from a UAV view. The focus is on human identification 
from an aerial view. To utilize this dataset with the popular YOLO models by Ultralytics (https://www.ultralytics.com/), the SynPlay dataset must be properly prepared. Specifically for my purposes, 
I need the 2D BBX annotations. Steps to perform this reformatting of SynPlay are: 

1. Rename all .txt Annotation files the same as the .jpeg Image files.
2. Move all Annotations into a "labels" folder.
3. Move all images into an "images" foder.
4. Reformat the Annotations in the .txt files to just contain 2D BBX coordinates for each annotation.
5. Create a .yaml file to accompany these files
6. Combine the "images" folder, "labels" folder, & .yaml file to have a YOLO formatted dataset

