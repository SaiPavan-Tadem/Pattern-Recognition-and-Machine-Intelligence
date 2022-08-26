# Adaptive contrast enhancement and Data Augumentation for deep learning based Pneumonia detection.
This is an implimented project with the help of reference from original papers [Radiologist-Level Pneumonia Detection on Chest X-Rays with Deep Learning](https://arxiv.org/abs/1711.05225) and [Pneumonia Detection in chest X-ray images using Convolutional Neural Networks and Transfer Learning](https://www.researchgate.net/publication/342619947_Pneumonia_Detection_in_chest_X-ray_images_using_Convolutional_Neural_Networks_and_Transfer_Learning).you can also check [my project report here](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Report_PneumoniaDetection.pdf)
## Sample Images 
Please Collect the data set from [kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)-Chest X-Ray Images (Pneumonia).
The sample Image is shown below.
![Alt Text](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Images/SampleImage.png)
# Method
Images - > Preprocesing{data augumentation,Contrast ENhancement} ->Vgg16{Model}->classification results

# Preprocessing:
# a) Data augumentation
It includes image rotation,flipping and addtion of gaussian noise.The data set size is increased to good scale,the results are shown below.
![Alt Text](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Images/Tabel.png)
# b) Contrast Enhancement
**Gamma Contrast Enhancement:** It is is a nonlinear operation used to encode and decode luminance or tristimulus values in video or still image systems. Mathematically explined by the following formula.
**Gaussian Contrast Enhancement:** Its a Non-linear transformation function to enhance brightness and contrast.
**Brightness enhancement** It is a linear trasnformation which adjust the brightness of the image based on the given gain value,after that the image also undergoes thresholding operation.
![Alt Text](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Images/Contrast.png)
## Model and Hyperparameters:

![Alt Text](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Images/vgg16.png)


| Name     | Value |
| ---      | ---       |
|Batch size-training  | `   128      |
|Batch size-validation  | ` 128       |
|Batch size-testing  | `    8   |
|Number of epochs  | `      10   |
| Learning Rate      | \|   2e-4     |
## Results:
The final classification results are shown in below table.For more information please check the [my project report here](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Report_PneumoniaDetection.pdf)
![Alt Text](https://github.com/SaiPavan-Tadem/Pattern-Recognition-and-Machine-Intelligence/blob/main/Images/result.png)





