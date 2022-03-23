## What it is about ?
This is a covid xray diagnostic model proposed using convolution neural networks which can identify the x-ray as a covid affected or a normal xray.  

## Explainable AI
In general a machine learning model is called as a black box model, as the user cannot be able to know on what basis the model is predicting the output. As this is an application of medical diagnostic model it is very important and nessesary to know on what basis the model is predicting the output. Explainable AI is one such a thing which can say the user, the significant areas identified by the model which is responsible for the output. In this project an explainable AI framework called as LIME (Local Interpretable Model Agnostics) has been used to identify the significant features that the model has identified.

## LIME (LOCAL EXPLAINABLE MODEL AGNOSITCS): 
LIME is an algorithm that can explain the predictions of any classifier or regressor in a faithful way, by approximating it locally with an interpretable model. LIME can be applied with any type of data classifications like TabularData, SemanticData, ImagesData and so on. In this project LIME is applied on an Image classification technique which helps in understanding the feature extractions by the model. LIME follows the steps given below for explaining the image classification model. 
#### 1. Generating the random perturbations as shown below
#### 2. Generation of various samples of perturbed images
#### 3. Making the model to work on the generated sample
#### 4. Computing the weights of each and every super pixel
#### 5. Building a linear classifier
#### 6. Highlights the superpixel with top coefficients
![image](https://user-images.githubusercontent.com/102225400/159691724-dd3d0345-27a5-4d84-bb01-53f177627663.png)
![image](https://user-images.githubusercontent.com/102225400/159691745-1516bb9e-609c-44b1-bb8b-3b2221f41066.png)
