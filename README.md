# Probabilistic U-Net Segmentation of Ambiguous Images:
- People with pulmonary disease often have a high opacity, which makes segmentation of the lung from chest X-rays more difficult.
- In this study, I propose a methodology to improve the performance of the U-NET structure so that it is able to extract the features and spatial characteristics of the X-ray images of the chest region, in addition to the ability to find a link between the left and right parts of the chest region, which helps the neural network to locate the lungs within the X-ray images ( segmentation).
- Since the variational autoencoder is used for generation, we can use it to extract the most important information in the x-ray images, such as what we mentioned, the relationship between the left and right parts of the chest region.
- Therefore, I proposed integrating the U-NET structure with the variational autoencoder structure in order to reach a neural network structure capable of segmentation for people with lung diseases.
- To ensure the accuracy of the study, the neural network was trained on medical chest x-rays of people with lung opacity, and then the model was tested on chest x-rays of people with COVID-19.
- The results were as follows: The model was able to train it on chest x-rays of people with lung opacity: accuracy: 0.9818 - precision: 0.9931 - recall: 0.9539. After completing the training, the model was tested on chest X-rays of people infected with COVID-19, and the results obtained were accuracy: 0.9782 - precision: 0.9886 - recall: 0.9613.

![download - 2023-02-08T224156 794](https://user-images.githubusercontent.com/108609519/217646464-3eb72e30-5a73-4a3d-bf28-fe7261072958.png)

The previous image shows several samples of X-ray images of a healthy person, a person with medium opacity, and a person with high opacity.

# Evaluation of the performance of the model:
## Evaluation of the performance of the model on x-rays of the chest area of people with lung_opacity:
![image](https://user-images.githubusercontent.com/108609519/217647360-74bd8542-6356-4503-9f7d-c12239cc8447.png)

## Evaluation of the performance of the model on x-rays of the chest area of people with covid:
![image](https://user-images.githubusercontent.com/108609519/217647444-5963e966-92c5-4c8d-93f0-b467c994f1b8.png)

# Compare original masks with those predicted by the model:
## Samples of Lung_opacity Images:

![Untitled (1)](https://user-images.githubusercontent.com/108609519/217750404-11a62279-8e70-4a1b-968c-691f8df1ab4e.jpeg)

## Samples of COVID-19 Images:

![Untitled](https://user-images.githubusercontent.com/108609519/217749635-2d31f033-871c-42c6-a25d-8b31e276be41.jpeg)

