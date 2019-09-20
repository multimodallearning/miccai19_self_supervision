In order to evaluate the expressiveness of different image descriptor types, we indirectly compare all feature extraction methods.
Therefore, we make use of the manually annotated VISCERAL Anatomy3 goldcorpus data for contrast-enhanced CT scans.
We split this dataset into 2 groups: labeled and unlabeled data.
Assuming, we have *n* labeled atlas images, for our unlabeled volume scans, we assign organ labels based on feature similarities when comparing their feature representations to those generated for the atlas images.

In our work, we extract feature descriptors at every 4th voxel inside the volume scans for every method.
To assign labels to these voxels, we rely on an approximate k-Nearest-Neighbor (kNN) search, that we introduced in our MICCAI 2016 submission (1) - [Vantage Point Forests](http://mpheinrich.de/code/vpForest_public.zip).


(1): Heinrich, Mattias P., and Maximilian Blendowski. "Multi-organ segmentation using vantage point forests and binary context features." International Conference on Medical Image Computing and Computer-Assisted Intervention. Springer, Cham, 2016.
