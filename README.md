# Deep-Learning-for-Automated-Identification-of-Plant-Leaf-Diseases
 
Introduction:
The agriculture sector in Kenya is essential, contributing 20% to the GDP and indirectly affecting another 27% through related sectors. It employs over 40% of the total population and 70% of rural inhabitants. Recognizing its importance in providing livelihoods and food, the Central Bank of Kenya launched the Survey of the Agriculture Sector in July 2022. This survey, alongside the CEOs and Market Perceptions Surveys, aims to generate frequent data to inform food supply, prices, and agricultural challenges, thereby supporting monetary policy decisions.

The Economic Survey of 2022 revealed a slowdown in agricultural growth, from 5.2% in 2020 to a 0.1% contraction in 2021, mainly due to unfavorable weather, reducing crop and livestock performance. Maize production fell from 42.1 million bags in 2020 to 36.7 million in 2021, with similar trends in beans, coffee, wheat, and tea. Factors like rising input costs, leaf rust infestation, and land use shifts to real estate contributed to this decline. In 2022, the sector contracted further in the first three quarters.

The January 2023 Agriculture Sector Survey focused on recent trends in agricultural commodity prices and outputs across the country. It also assessed key food commodity availability. The survey's areas of interest included tracking commodity prices, assessing output and acreage, farm input usage, factors affecting production.

The improvement of crop yields in Kenya through technology is a critical issue, given that small farmers, who own less than five acres each, constitute up to 75% of the country's agricultural workforce. These farmers traditionally rely on outdated methods and lack access to modern technologies that could enhance productivity and ease their labor.

Challenges in Enhancing Farming Productivity:

Small farmers face significant challenges due to their reliance on traditional farming methods.
There is a pressing need to integrate modern technology into agriculture to increase crop yields, improve income, and reduce labor hours.

Advantech's "Farming as Business" program aims to provide data and decision-making tools to farmers in East Africa.
They offer a smartphone app providing advanced weather forecasts, market trends, and information on soil types, fertilizers, and pesticides, helping farmers make data-driven decisions.

We are working on developing a Convolutional Neural Network (CNN) model for Advantech's mobile app, aimed at helping farmers diagnose plant diseases through image recognition, involves several steps. This model would leverage the power of machine learning and image processing to identify various plant diseases from photos taken by farmers. This model will help in accurate and timely detection of plant diseases which plays a crucial role in ensuring food security and sustainability. With the advent of precision agriculture and the application of AI in this field, there is an opportunity to develop automated systems for early disease detection in crops. 

CITATIONS
Kenya Agricultural & Livestock Research Organization. (n.d.). Improving Crop Yield Using Technologies. Retrieved from https://www.kari.org/improving-crop/
Kenya Agribusiness and Agroindustry Alliance. (n.d.). Challenges Facing the Agricultural Sector in Kenya. Retrieved from http://kaaa.co.ke/challenges-facing-the-agricultural-sector-in-kenya/
UK Government. (n.d.). Agricultural Productivity in Kenya: Barriers and Opportunities. Retrieved from https://www.gov.uk/government/publications/agricultural-productivity-in-kenya-barriers-and-opportunities

Objective:
The primary objective of this project is to develop a 9-layer deep CNN capable of accurately classifying 39 different classes of plant leaf diseases, as well as distinguishing healthy leaves and background without leaves. The project aims to create an efficient and reliable model that can be used for automated disease detection in agricultural applications.

Dataset Description:
The dataset comprises 61,486 images across 39 classes, including various diseases affecting apple, blueberry, cherry, corn, grape, orange, peach, pepper, potato, raspberry, soybean, squash, strawberry, and tomato plants. The dataset has been enhanced using six different augmentation techniques: image flipping, Gamma correction, noise injection, PCA color augmentation, rotation, and scaling.

Methodology:

Data Preprocessing:

Perform additional image preprocessing as needed.
Split the dataset into training, validation, and testing sets.
Model Development:

Design and implement  CNN.
Experiment with different layer configurations and hyperparameters to optimize the model.
Model Training and Validation:

Train the model using the training set.
Validate and tune the model using the validation set to avoid overfitting.
Model Evaluation:

Evaluate the model's performance on the test set using metrics like accuracy, precision, recall, and F1-score.
Deployment Strategy:

Plan the integration of the model into a practical application for use in agricultural settings.
Expected Outcomes:

A highly accurate and reliable CNN model for the classification of plant leaf diseases.
A comprehensive report detailing the model's performance, limitations, and potential applications.

Conclusion:
This project seeks to leverage the power of deep learning in the field of agriculture, specifically in the area of plant disease identification. The successful completion of this project could significantly improve disease management in crops, leading to better agricultural practices and increased yields.
