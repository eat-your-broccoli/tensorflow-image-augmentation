# tensorflow-image-augmentation
A simple docker container to run jupyter notebooks for image augmentation for machine learning.

The images are loaded from `srcImg`, scaled down and saved to `downscaledImg`, then augmented and saved to `augmentedImg`. 

## Start
run `docker-compose up`

or for starting in background 
run `docker-compose up -d`

## Adding Images

Place your images in subfolders of `srcImg`. The subfolders' names are the class names.

```
data
-| srcImg
---| class1
-----| img.jpg
-----| img2.png
---| class2
-----| img1.jpg
-----| img2.png
```
