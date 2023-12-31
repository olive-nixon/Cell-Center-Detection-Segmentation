# Cell-Center-Detection&Segmentation
Detecting the location and draw boundary of nuclei from tissue microscopic images (H&E stained).
Model is based on U-net with contour enhancement in loss function. Overlap patch based strategy is used to 1) adapt to variant input image size (resize image may stretch features); 2) use random clip and rotation for data augmentation; 3) each region in output mask is determined by combining inference result from multiple patches. More details can be found in [1].
 
### Dependencies
- Tensorflow
- OpenCV
- Scikit-image
- Numpy
- Pandas
- Matplotlib

#### More
- [x] detection and segmentation model
- [x] consider edge into loss function during training
- [x] morphology operation to calculate center and boundary
- [ ] better color normalization method for preprocess
- [ ] identify overlapping samples with local segmentation model
- [ ] identify tissue types 
