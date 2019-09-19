################################################################################################
This repository contains code and a description of the data preprocessing pipeline for our work 

"How to learn from unlabeled volume data: Self-Supervised 3D Context Feature Learning"
published at the MICCAI 2019 conference in Shenzhen, China.

################################################################################################

Find our paper here: <TODO: insert springer URL>

The overall process basically contains 3 major blocks:
1) preprocessing the VISCERAL data set
2) training of several CNN architectures 
3) evaluating the image descriptors by organ labeling using an approximate kNN-search  

For the first and last step, we provide detailled descriptions in the according txt-files.
The training procedures for our proposed feature extractor CNNs is provided in form of a jupyter notebook.
