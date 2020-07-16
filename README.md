# Detecting-Deepfakes-with-OpenCV
This project involves usage of computer vision methods and machine learning model to detect if the image is fake or not

## Dataset Used:
[VidTMIT](https://liveproject-resources.s3.amazonaws.com/other/detectingdeepfakes/VidTIMIT.zip) and [DeepFakeTMIIT](https://liveproject-resources.s3.amazonaws.com/other/detectingdeepfakes/DeepfakeTIMIT.tar.gz) Dataset was used for this project where deefake contains fake images created from the original videos of VidTIMIT

## Methodology
1. Read/write a single image frame from videos, compute differences between fake and real frames, and compute histograms.
2. Detection and cropping faces from the images as faces are the maine objective of this project
3. Compare two different faces using diffrent measures like histogram,feature matching,Template matching,SSIM,PSNR,MSE,AD etc
4. Created a datatset Train(80%) and Test(20%) combing all the feature vectors of fake and real images and labelled them as 0 and 1
5. Implemented SVM with Linear kernal which outperformed all the other kernels

## Result
F1 Score : 0.92


Resources:
1. https://realpython.com/face-recognition-with-python/
2. https://machinelearningmastery.com/how-to-perform-face-detection-with-classical-and-deep-learning-methods-in-python-with-keras/
3. https://www.pyimagesearch.com/2017/05/22/face-alignment-with-opencv-and-python/
4. https://abndistro.com/post/2019/07/07/detecting-image-differences-using-python-and-opencv/
5. https://www.pyimagesearch.com/2014/09/15/python-compare-two-images/
6. https://towardsdatascience.com/feature-selection-techniques-in-machine-learning-with-python-f24e7da3f36e
7. https://www.newbedev.com/python/howto/how-to-iterate-over-files-in-a-given-directory/
8. https://towardsdatascience.com/evaluating-machine-learning-classification-problems-in-python-5-1-metrics-that-matter-792c6faddf5
9. https://rpubs.com/Sharon_1684/454441
