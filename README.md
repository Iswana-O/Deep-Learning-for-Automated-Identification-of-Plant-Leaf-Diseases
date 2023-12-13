# Deep-Learning-for-Automated-Identification-of-Plant-Leaf-Diseases
 The agriculture sector in Kenya is essential, contributing 20% to the GDP and indirectly affecting another 27% through related sectors. It employs over 40% of the total population and 70% of rural inhabitants. Recognizing its importance in providing livelihoods and food, the Central Bank of Kenya launched the Survey of the Agriculture Sector in July 2022. This survey, alongside the CEOs and Market Perceptions Surveys, aims to generate frequent data to inform food supply, prices, and agricultural challenges, thereby supporting monetary policy decisions.

The Economic Survey of 2022 revealed a slowdown in agricultural growth, from 5.2% in 2020 to a 0.1% contraction in 2021, mainly due to unfavorable weather, reducing crop and livestock performance. Maize production fell from 42.1 million bags in 2020 to 36.7 million in 2021, with similar trends in potatoes, beans, coffee, wheat, and tea. Factors like rising input costs, leaf rust infestation, and land use shifts to real estate contributed to this decline. In 2022, the sector contracted further in the first three quarters.

The January 2023 Agriculture Sector Survey focused on recent trends in agricultural commodity prices and outputs across the country. It also assessed key food commodity availability. The survey's areas of interest included tracking commodity prices, assessing output and acreage, farm input usage, and factors affecting production.

The improvement of crop yields in Kenya through technology is a critical issue, given that small farmers, who own less than five acres each, constitute up to 75% of the country's agricultural workforce. These farmers traditionally rely on outdated methods and lack access to modern technologies that could enhance productivity and ease their labor.


## Challenges in Enhancing Farming Productivity

Small farmers face significant challenges due to their reliance on traditional farming methods.
There is a pressing need to integrate modern technology into agriculture to increase crop yields, improve income, and reduce labor hours.

Advantech's "Farming as Business" program aims to provide data and decision-making tools to farmers in East Africa.
They offer a smartphone app providing advanced weather forecasts, market trends, and information on soil types, fertilizers, and pesticides, helping farmers make data-driven decisions.

Agriculture, a cornerstone of human sustenance, has embraced technological advancements to bolster productivity and address challenges. In this vein, the proposed project delves into the realm of plant health, specifically the early identification of leaf diseases. Acknowledging the pivotal role of timely disease detection in safeguarding crop yield, we aim to leverage deep learning, employing a deep convolutional neural network (CNN). This venture is fueled by a dataset meticulously compiled by Arun Pandian J and Geetharamani Gopal

This project seeks to leverage the power of deep learning in the field of agriculture, specifically in the area of plant disease identification. 
We are working on developing a Convolutional Neural Network (CNN) model for Advantech's mobile app, aimed at helping farmers diagnose plant diseases through image recognition, which involves several steps. 


This model would leverage the power of machine learning and image processing to identify various plant diseases from photos taken by farmers. This model will help in the accurate and timely detection of plant diseases which plays a crucial role in ensuring food security and sustainability. With the advent of precision agriculture and the application of AI in this field, there is an opportunity to develop automated systems for early disease detection in crops. The successful completion of this project could significantly improve disease management in crops, leading to better agricultural practices and increased yields.

Project Objective
The primary objective of this project is to develop a CNN model capable of accurately classifying different classes of potato plant leaf diseases, as well as distinguishing healthy leaves and unhealthy leaves. The project aims to create an efficient and reliable model that can be used for automated disease detection in agricultural applications

Methodology
Data Preprocessing: Perform additional image preprocessing as needed. Split the dataset into training, validation, and testing sets.

Model Development: Design and implement CNN. Experiment with different layer configurations and hyperparameters to optimize the model.

Model Training and Validation: Train the model using the training set. Validate and tune the model using the validation set to avoid overfitting.

Model Evaluation: Evaluate the model's performance on the test set using metrics like accuracy, precision, recall, and F1-score.

Deployment Strategy: Plan the integration of the model into a practical application using StreamLit where users will be able to upload images of their leaves and get a diagnosis of the plant.

Expected Outcomes: A highly accurate and reliable CNN model for the classification of plant leaf diseases. A comprehensive report detailing the model's performance, limitations, and potential applications.

## DATA PREPROCESSING
Augmentation vs. No Augmentation
Our dataset comprises two sets of images: one with augmentation and another without. In the absence of augmentation, images maintain their original form, resulting in limited dataset diversity and an elevated risk of overfitting.

In contrast, augmented images undergo transformations, promoting greater diversity, improved generalization to new data, and a reduction in overfitting.

The advantages of augmentation include enhanced generalization, increased model robustness across different patterns, and improved data efficiency by expanding the dataset without the need for additional data collection; a particularly valuable asset in resource-constrained scenarios. For our work, we will utilize images with augmentation.

## EXPLORATORY DATA ANALYSIS
Since we were working with images the EDA involved various techniques to understand and analyze the characteristics and patterns within our image dataset.

## VISUAL INSPECTION
A subset of images was visually inspected to understand the general characteristics, such as color distribution, presence of noise, and overall image quality.  We had 3 classes as per the below image Potato early blight, Potato Late blight, and Potato healthy.

## MODEL ARCHITECTURE.
### Basic Model - CNN
Our CNN model will use ReLU to introduce non-linearity and capture complex patterns in hidden layers and a Softmax output layer to convert raw scores into class probabilities for multi-class classification.

### Deep CNN Models
From the basic CNN model we added 11 more layers to enforce deep learning. 

### GoogleNet's Inception Model.
This method ensures efficient feature extraction with its inception modules, reducing parameters for computational efficiency. Its multi-pathway design captures diverse features, providing a broader receptive field and enabling effective representation learning.
By augmenting this base with a Global Average Pooling layer and a Dense layer employing softmax activation for classification, the model adapts its knowledge to the task of identifying potato leaf diseases.
An EarlyStopping callback is implemented to curb overfitting and ensure optimal generalization during the training process.

## MODEL DEPLOYMENT
For the deployment of our models, we were using Google Cloud Platform (GCP) and Streamlit. We developed a Streamlit app that will act as the interface for our models. Used Python to develop the script. Find the link here: https://predict-ipwknoicua-uc.a.run.app

We deployed the Streamlit app on a GCP service -App Engine . For App Engine, we created an app.yaml file to configure the deployment. 

RECOMMENDATIONS AND CONCLUSIONS
Base CNN Model:

The Base CNN Model has delivered outstanding results by achieving a remarkably high validation accuracy of 96.54% in the intricate task of classifying potato leaf diseases. This significant accuracy underscores the model's proficiency in accurately identifying and categorizing diverse instances of potato leaf ailments. The achievement of such a high accuracy rate is indicative of the model's robust ability to detect abnormal patterns and features associated with different disease states in potato plants.

While the overall performance is promising, it is crucial to acknowledge and address the observed variations in accuracy across distinct disease classes. The model's ability to correctly identify specific diseases might be subject to fluctuations, necessitating a closer examination of its performance at a granular level. Understanding and mitigating these variations are pivotal steps in ensuring the model's reliability across the spectrum of potato leaf diseases.

Deep CNN Model:



Inception Model:

The Inception Model has demonstrated commendable performance, achieving a validation accuracy of 93.57% in classifying potato leaf diseases. This accuracy signifies the model's effectiveness in extracting distinctive features relevant to disease patterns, albeit slightly lower compared to the Base CNN Model. The marginal difference in accuracy suggests that the Inception Model could potentially offer an alternative and complementary approach to feature extraction.

To further enhance the Inception Model's accuracy, the recommendation is to embark on a fine-tuning process. Fine-tuning involves adjusting the model's hyperparameters or training on additional data to optimize its performance. This targeted optimization process aims to narrow the accuracy gap and potentially surpass the performance of the Base CNN Model. By understanding these challenges, the fine-tuning process can be more informed, addressing the root causes of misclassifications and bolstering the model's overall predictive capability.


Recommendations and Future Work

In enhancing the potato leaf disease detection project, we strongly recommend the inclusion of a non-leaf class to address scenarios where the input may not be a diseased leaf. This addition will significantly improve the model's versatility, allowing it to distinguish non-leaf objects effectively. To implement this, it is crucial to design a diverse dataset representing various non-leaf instances and modify the model architecture to accommodate the new class. Fine-tuning the model on this augmented dataset will enable it to detect features associated with non-leaf objects. This strategic expansion will not only broaden the model's applicability but also contribute to a more comprehensive understanding of the broader context in which potato leaf disease detection operates.

Diversifying the negative class data is a critical step in refining the model's ability to distinguish features specific to potatoes, thereby minimizing the risk of misclassifying non-potato images. By incorporating a broader range of negative examples, the model gains exposure to a more comprehensive set of non-potato instances. This diversification facilitates a more nuanced understanding of what constitutes a non-potato object, reducing the chances of false positives and enhancing the model's overall robustness. The inclusion of varied non-potato images ensures that the model can better discriminate between potato-related features and those unrelated to the domain, ultimately improving the accuracy and reliability of the potato leaf disease detection application.

 
