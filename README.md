## Real time Covid Xray diagnostics
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

## Architectures Used
In this project different CNN Architectures like DelNet, Inception, Nasanet, Mobilenet, VGG16 are used to evaluate the proposed model. The architectures of each cnn model are shown below: 
### 1. Proposed CNN Architecture: 
In the proposed cnn architecture a total of 8 layers for Feature extraction, 1 hidden layer, 1 output layer with Sigmoid activation function has been used. 

![image](https://user-images.githubusercontent.com/102232692/159826027-b07906bf-5467-415d-af2e-3f0a3c75962f.png)

The model ended up with a training accuracy of 92%. 
### 2. Inception Architecture: 
Generally, InceptionV3 is 48 layers deep. In this project those 48 layers are used for feature extraction and in the fully connected layer 1 hidden layer and an output layer has been kept. The InceptionV3 model is trained by making the feature extraction layers as untrainable. The architecture of the inception V3 model is as shown below. 

![image](https://user-images.githubusercontent.com/102232692/159826794-01f25bdd-c9b0-457c-bd47-0c1381f4b462.png)

![image](https://user-images.githubusercontent.com/102232692/159826899-a60faab8-015f-48ce-931f-eccfca532a45.png)

### 3. DenseNet201: 
Generally Densenet201 model is 201 layers deep. In this project those 201 layers are used for feature extraction and in the fully connected layer 1 hidden layer and an output layer has been kept. The Densenet201 model is trained by making the feature extraction layers as untrainable

![image](https://user-images.githubusercontent.com/102232692/159827514-270cb2e8-b0ac-466a-9c04-e2e41ea159c4.png)

![image](https://user-images.githubusercontent.com/102232692/159827884-41c0e09e-f240-44b6-8811-bf0061c6e226.png)


