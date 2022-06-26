# HumpbackWhaleClassification
Humpback Whale Identification using CNN and CAM to understand Whale population dynamics - Image Processing Project (CSE 4019)

## Abstract
After centuries of intense whaling, recovering whale populations still have a hard time adapting to warming oceans and struggle to compete every day with the industrial fishing industry for food. In some areas of the Northern Pacific Ocean, Whales are also being hunted for their skin and fat. The Humpback Whale is also currently identified as an endangered species by the International Union for Conservation of Nature. It is important to keep a consensus of these species. Since these are extremely large mammals, it is hard to find mechanisms to count. Oceanographers capture pictures of Whales everytime they surface. These pictures are used to estimate their population per square kilometer. In the interest of making conservation efforts for the Whale population, it is important to understand and analyse their population dynamics, This paper aims to uniquely identify whales for this purpose. The above is carried out using Transfer Learning approaches for classification after preprocessing the images for foreground extraction and visualizing the localisation of feature mappings using Class Activation Maps(CAM). The paper also focuses on the comparative analysis of these transfer learning techniques and the impact that foreground extraction and pre-processing techniques have on image classification and feature localisation for identification of the whale. Current existing methods only focus on achieving higher accuracies with deeper network architectures, for classification while this paper first focuses on Whale fluke localisation using CAM and then uses a Deep Learning model. There is currently no such existing technique that uses Foreground Extraction on whale flukes to get the sea and sky background out of the way. Our Method uses CAM to show that there is a clear difference before and after Foreground Extraction.

#### Keywords
Image Segmentation, Convolutional Neural Networks, Transfer Learning, Class Activation Maps, Image Enhancement

## Foreground Extraction Process
<img src="https://github.com/anishsghiya/HumpbackWhaleClassification/blob/main/Images/Foreground%20Extraction.png" alt="drawing" width="250"/>

## Results
<img src="https://github.com/anishsghiya/HumpbackWhaleClassification/blob/main/Images/Output_img.png" alt="drawing" width="300"/>


| Model Name    | Keras Preprocessing | Foreground Extraction  | ForegroundExtraction + KerasPre-processing |
| ------------- |---------------------| -----------------------|--------------------------------------------|
| ResNet50      | 0.5556  | 0.6263 | 0.6364
| VGG16         | 0.61616 | 0.6767 | 0.7879
| InceptionResNetV2 | 0.5353 | 0.6868 | 0.7374
| VGG19         | 0.62626 | 0.74747| 0.7894 

## Author
Anish Ghiya, Vaibhav Vijay, Aditi Ranganath
