For our experiments, we use the contrast-enhanced thoracoabdominal CT scans of the VISCERAL Anatomy3 data set (1). 
Follow the instructions at the challenge website [VISCERAL Anatomy3](http://www.visceral.eu/benchmarks/anatomy3-open/) to get access to this data.

We perform the following steps to preprocess the silvercorpus data and subsequently the goldcorpus with its manually annotated organ labels.

1) At first, we isometrically resample a total of 63 silver corpus patients to a resolution of 1.5mm^3. We exclude two patients (IDs: 10000107, 10000157) since there are obvisously recontruction issues, when inspecting these volume scans.

2) We proceed to resample the respective organ segmentations to the same voxel spacing (labels IDs: '58', '86', '29662', '29663', '32248', '32249'; i.e. liver, spleen, left & right kidney, left & right psoas major muscle). 

3) Compute the center of mass (COM) for an organ mask of 6 foreground structures to crop the images to a common region of interest. Note that we use the silvercorpus annotations here only to compute the COMs. During the pretraining later on, the annotation quality of these labels does not matter, since our method only relies on spatial relations and does NOT use any label information.
    - awda
    - awda

(1): Jimenez-del-Toro, Oscar, et al. "Cloud-based evaluation of anatomical structure segmentation and landmark detection algorithms: VISCERAL anatomy benchmarks." IEEE transactions on medical imaging 35.11 (2016): 2459-2475.
