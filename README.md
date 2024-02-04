# HackathonProject
Fraudalent image classification of car insurance claims

Problem Statement
Within the realm of insurance, the processing of claims related to vehicle damage stands out as a routine yet crucial responsibility. The insurance sector grapples with an ongoing dilemma in distinguishing genuine claims from deceptive ones, a situation that can result in substantial financial setbacks. The emergence of Generative AI and various stable diffusion models has contributed to a surge in the number of fraudulent claims. It has become commonplace for users to incorporate fraudulent images as components of the claim settlement process.

This poses a formidable challenge to insurance companies as they strive to differentiate between legitimate and deceitful claims. Deceptive claims often involve amplifying the severity of damage or fabricating entirely false claims. To curb these financial losses and uphold the integrity of their operations, insurance firms must formulate effective approaches for accurately and efficiently flagging fraudulent claims.

In the context of this hackathon, the WNS team invites the community to devise a robust and high-performance model utilizing computer vision techniques to classify images as either fraudulent or non-fraudulent within the context of insurance claims. By precisely identifying fraudulent images, insurance companies can evaluate the authenticity of a claim and make well-informed decisions regarding payout.


Dataset
You are provided with 3 files: training set, test set and sample submission.

The training set contains a diverse dataset of car images, each labeled with information being fraudulent or non fraudulent. The dataset includes images from varying lighting conditions, cluttered backgrounds, long tail distribution, and so on.

In the test set, you are provided with only the images and you need to predict the label as fraudulent or non fraudulent for each image present.

The sample submission file contains the format in which the user needs to submit the solution file.


Dataset Description
Following is the dataset description of training set, test set and sample submission.


Training set
The training set contains 2 files: images folder and train.csv

The images folder contains the images which are to be used for training the model and train.csv contains the labels of each image present in the training set and data description is given below.

Column Name	Description
image_id	Unique identifier of the row
filename	Name of the image
label	Binary variable containing 0 or 1. 0 indicates non-fraudulent claim and 1 indicates fraudulent claim
 

Test set
The test set contains 2 files: images folder and test.csv

The images folder contains the test images for which prediction is to be done and test.csv contains the unique identifiers of each image present in the test set. You will need to make predictions for each image present in the test set and data description is given below.

Column Name	Description
image_id	Unique identifier of the row
filename	Name of the image

Sample Submission 
Sample submission contains 2 columns - image_id and label and its description is given below

Variable

Description

image_id

Unique identifier of an image

label 

Binary variable containing 0 or 1. 0 indicates non fraudulent claim and 1 indicates fraudulent claim

 

Evaluation metric
The model will be evaluated with the macro F1 score.


