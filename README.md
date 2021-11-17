# tensorflow-image-augmentation
A simple docker container to run jupyter notebooks for image augmentation for machine learning.

Two jupyter notebooks exist. One loads images from `srcImg`, scales them down to below 0.5MB, and then saves to `downscaledImg`.
The other notebook loads the images from `downscaledImages`, augments them (flip, rotate, shift, zoom, ...) and then saves them to `augmentedImg`.

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
