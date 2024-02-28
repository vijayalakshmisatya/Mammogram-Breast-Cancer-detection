# Mammogram-Breast-Cancer-detection


## Overview
Among many cancers, breast cancer is the second most common cause of death in women. Early detection and early treatment reduce breast cancer mortality. Mammography plays an important role in breast cancer screening because it can detect early breast masses or calcification regions.

## Signs of Breast Cancer:
1. Weight loss
2. Skin changes
3. Pain
4. Breast changes
This project uses mammograms for breast cancer detection using deep learning techniques.

For the diagnosis of breast cancer doctors often use additional tests to find or diagnose breast cancer. A mammogram is an X-ray picture of the breast. Doctors use a mammogram to look for early signs of breast cancer. Regular mammograms are the best tests doctors have to find breast cancer early, sometimes up to three years before it can be felt. A mammogram shows how dense the breasts are. Women with dense breasts have a higher risk of getting breast cancer.

## Dataset
dataset is a preprocessed version of the original MIAS (Mammographic Image Analysis Society) dataset. It contains 1,679 images with the labels:
normal (0)
benign (1)
malignant (2).

All images were preprocessed by removing artifacts, such as labels and enhancing the images using CLAHE (Contrast Limited AHE). For abnormal images (benign and malignant), the region of interest (ROI) was extracted using the x/y coordinates and radius provided by the original MIAS dataset, and a central breast area was used for normal images.
All training images were augmented to increase the dataset size by using rotation (90°, 180°, 270°), vertical flipping, random bightness and contrast changes, augmenting the training data by a factor of 16. Finally, the training dataset was balanced, resulting in 528 training images per class.
The dataset consists of a total of 1584 training images, 47 validation images, and 48 testing images.
The images were resized to 224 x 224 pixels and are available in .npy format.

## Image Processing
Since the mammograms looks blury and dull, image preprocessing has been done to increase the sharpness and contrast of the image.
![Screenshot_665](https://github.com/vijayalakshmisatya/Mammogram-Breast-Cancer-detection/assets/159516375/98df505a-603e-43e9-bd4e-af8d18c4ed07)


## Why Deep-Learning?
AI system studying X-ray mammograms was shown to be better than human experts when it came to predicting whether or not a patient has breast cancer. More specifically, the model was found to be as good as two doctors looking at the images, and better at spotting cancer than a single doctor, while also reducing the number of “false-negative” results. Such systems will never replace medical staff, but would serve as an extra set of eyes, while also being able to work 24/7 without getting tired or making mistakes.
