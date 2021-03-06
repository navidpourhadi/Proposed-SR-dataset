
# Super-Resolution(SR) dataset

In this repository, we propose and provide a dataset of Persian License-Plates(LP) which can be employed to train the SR systems. The dataset contains both High-Resolution(HR) and Low-Resolution(LR) images that are needed for training an SR network. 

## procedure of preparation

The SR-dataset contains about 6000 pair images of Persian LPs. The HR images are derived from the [ALPR dataset](https://github.com/behnoudshafizadeh/iranian-LPR-using-deep-learning-algorithm). As it was mentioned above, the images were captured in different circumstances with different qualities. Then we resized all the images to the same size (192,68) for better performance.

Because the process of capturing two HR and LR images of a scene (LPs of cars) with two cameras is so hard and impractical (both images must cover same area of scene without any difference in the arrangement and position of objects), we had to generate the LR license-plate images synthetically from mentioned HR license-plate images. 
To closely mimic reality, a random down-scaling is utilized. In the process of generating LR images, the corresponding HR image is haphazardly resized (to a size lower than the required LR image’s). Then, the resulted resized image is up-scaled to match the target LR-image’s size.

## Structure of dataset

The SR-dataset is composed of 6000 HR images of LPs with their correspond 2X and 4X LR images. Also, the dataset is splited to 5000, 500, and 500 images for training, validation, and test, respectively.

                    
   Category   |   Percentage  |  number of images
------------- | ------------- | -------------
Train  | 83%  | 5000
Validation  | 8.3%  | 500
Test  | 8.3%  | 500

## Samples of Dataset

   HR image   |   2X LR image  |  4X LR image
------------- |  ------------- | -------------
<img src="/samples/0001HR.jpg"  width="192" height="68">  | <img src="/samples/0001X2.jpg"  width="192" height="68">  | <img src="/samples/0001X4.jpg"  width="192" height="68">
<img src="/samples/0002HR.jpg"  width="192" height="68">  | <img src="/samples/0002X2.jpg"  width="192" height="68">  | <img src="/samples/0002X4.jpg"  width="192" height="68">
<img src="/samples/0004HR.jpg"  width="192" height="68">  | <img src="/samples/0004X2.jpg"  width="192" height="68">  | <img src="/samples/0004X4.jpg"  width="192" height="68">


## Accessing the dataset
For accessing the full version of dataset, please contact us:
emails:
  - npourhadi1998@gmail.com
  - behnoud.shafizadeh@gmail.com



## Authors

- [Navid Pourhadi](https://www.github.com/navidpourhadi)
- [Behnoud Shafizadeh](https://github.com/behnoudshafizadeh)
