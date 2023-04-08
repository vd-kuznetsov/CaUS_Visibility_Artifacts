# CaUS_Visibility_Artifacts
 Repository for the paper "Neural Networks for Classification and Unsupervised Segmentation of Visibility Artifacts on Monocular Camera Image" 

## Dataset 

Dataset "VisibilityArtifacts" consists of a partial combination of images from the data sets:
1. [Woodscape](https://woodscape.valeo.com/) ("Soiling Detection" sample), radial distortion has been eliminated for this set and the images have been corrected;
2. [DrivingStereo](https://drivingstereo-dataset.github.io/) ("Different weathers" sample);
3. [TapmerDetection](https://www.researchgate.net/publication/329463231_Visibility_Loss_Detection_for_Video_Camera_Using_Deep_Convolutional_Neural_Networks_Volume_1).
4. [ACDC](https://acdc.vision.ee.ethz.ch/);

In order to balance the number of images per class, data augmentation was performed using the [imgaug](https://github.com/aleju/imgaug) tool, from thoseimages in which there were no visibility artifacts. As a result, a balanced "VisibilityArtifacts" dataset was formed, including 22311 images, divided into 7 categories, it's description is given in Table 2, examples of images are shown in Fig. 2 in the article.

If you want to use this dataset in your research, then read the following conditions:
1. [Woodscape license](https://drive.google.com/file/d/12IrLnGfng6s-NogJLIvUZsCxF1NDA-FA/view?usp=sharing);
2. [DrivingStereo license](https://github.com/drivingstereo-dataset/drivingstereo-dataset.github.io/blob/master/LICENSE);
3. [ACDC license](https://acdc.vision.ee.ethz.ch/contact).

Because if you download the dataset "VisibilityArtifacts", then you accept them automatically.

Links to the dataset:
1. Classification: [part 1](https://drive.google.com/drive/folders/1AxqLHFCjtoDiJjD0lweiOzVuTDZgla3h?usp=share_link), [part 2](https://drive.google.com/drive/folders/15z3pimTCFH9ywO9oNgpGC6Ff_04Z4O_z?usp=share_link);
2. Segmentation: [part 3](https://drive.google.com/drive/folders/1Sls5GpqtiyXfC0BsfL3O6GNzAUcVbKfH?usp=share_link).

For comfortable data processing, use the code from the "Loading data and splitting it" section of the notebook "Training Classifiers.ipynb".
## Citation

```
@article{kuznetsov2022neural,
  title={Neural Networks for Classification and Unsupervised Segmentation of Visibility Artifacts on Monocular Camera Image},
  author={Kuznetsov, Vladislav I and Yudin, Dmitry A},
  journal={Optical Memory and Neural Networks},
  volume={31},
  number={3},
  pages={245--255},
  year={2022},
  publisher={Springer}
}
```
