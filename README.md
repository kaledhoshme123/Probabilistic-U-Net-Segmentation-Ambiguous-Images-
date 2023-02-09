# Probabilistic U-Net Segmentation of Ambiguous Images:
- People with pulmonary disease often have a high opacity, which makes segmentation of the lung from chest X-rays more difficult.
- In this study, I propose a methodology to improve the performance of the U-NET structure so that it is able to extract the features and spatial characteristics of the X-ray images of the chest region, in addition to the ability to find a link between the left and right parts of the chest region, which helps the neural network to locate the lungs within the X-ray images ( segmentation).
- Since the variational autoencoder is used for generation, we can use it to extract the most important information in the x-ray images, such as what we mentioned, the relationship between the left and right parts of the chest region.
- Therefore, I proposed integrating the U-NET structure with the variational autoencoder structure in order to reach a neural network structure capable of segmentation for people with lung diseases.
- To ensure the accuracy of the study, the neural network was trained on medical chest x-rays of people with lung opacity, and then the model was tested on chest x-rays of people with COVID-19.
- The results were as follows: The model was able to train it on chest x-rays of people with lung opacity: accuracy: 0.9829 - precision: 0.9939 - recall: 0.9606. After completing the training, the model was tested on chest X-rays of people infected with COVID-19, and the results obtained were accuracy: 0.9789 - precision: 0.9902 - recall: 0.9650.

![download - 2023-02-08T224156 794](https://user-images.githubusercontent.com/108609519/217646464-3eb72e30-5a73-4a3d-bf28-fe7261072958.png)

The previous image shows several samples of X-ray images of a healthy person, a person with medium opacity, and a person with high opacity.

# Evaluation of the performance of the model:
## Evaluation of the performance of the model on x-rays of the chest area of people with lung_opacity:
![image](https://user-images.githubusercontent.com/108609519/217879613-297095b9-17a5-4073-81c1-6377584e651b.png)


## Evaluation of the performance of the model on x-rays of the chest area of people with covid:
![image](https://user-images.githubusercontent.com/108609519/217879879-79bde87c-c13f-4df4-86e9-ce5a93f07127.png)

# Compare original masks with those predicted by the model:
## Samples of Lung_opacity Images:

![Untitled (3)](https://user-images.githubusercontent.com/108609519/217881317-7b3b227b-0a06-4eeb-b55c-1c55450d5fc1.jpeg)

## Samples of COVID-19 Images:

![Untitled (4)](https://user-images.githubusercontent.com/108609519/217881662-7b60c234-f842-4471-b486-2cf4fa1c818f.jpeg)

