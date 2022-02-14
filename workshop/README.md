# Full Workshop Title
Integrating Custom Vision with Power Apps for Diabetic Retinopathy Detection
## Module Source Link
https://docs.microsoft.com/en-us/learn/modules/classify-images-custom-vision/

https://docs.microsoft.com/en-us/learn/modules/customize-apps-in-powerapps/

## Goals

In this workshop, we will discuss how to build a no-code app with Custom Vision to classify imagines 

| **Goal**              |                     Description           |
| ----------------------------- | --------------------------------------------------------------------- |
| **What will you learn**       | How to build an app with Power Apps and integrate Custom Vision to classify imagines                                        |
| **What you'll need**          | [Custom Vision](https://www.customvision.ai/), [Power App]( https://make.powerapps.com)|
| **Duration**                  | 1 hour                                                                |
| **Just want to try the app or see the solution?** | *an optional link to the completed project sample app or solution folder*                          |
| **Slides** | [Powerpoint](slides.pptx) 
                         
## Video

Embed your Train the Trainer video here. Instructions on how to create a great video experience is [available on this page](../video-guidance.md).

## Pre-Learning

[Get started with Computer Vision](https://docs.microsoft.com/en-us/learn/modules/analyze-images-computer-vision/)

[Get started with Power App](https://docs.microsoft.com/en-us/learn/modules/get-started-with-powerapps/)

## Prerequisites

Ability to navigate the Azure portal
Familiarity with OneDrive, SharePoint, and Excel

## What students will learn

Do you want to customize an app by adding controls, images, and logic or create intelligent solutions that extract information from images, but just haven't started yet? If so, this workshop is what you'll need.

![image](https://user-images.githubusercontent.com/49314681/153230680-9351bded-4c7c-43e3-aa61-a9c5ae55f357.png)


## Milestone 1 - Custom Vision project build up

In this segment, you'll query an API at the Metropolitan Museum of Art

In Azure, you can use the Custom Vision cognitive service to train an image classification model based on existing images. There are two elements to creating an image classification solution. First, you must train a model to recognize different classes using existing images. Then, when the model is trained you must publish it as a service that can be consumed by applications.

1.Let's begin by getting a dataset of diabetic retinopathy images. 

2.open the Custom Vision portal at https://customvision.ai. If prompted, sign in using the Microsoft account associated with your Azure subscription and agree to the terms of service

3.In the Custom Vision portal, create a new project with the following settings:

    Name: Diabetic Retinopathy detection 
    
    Description: Image classification for Diabetic Retinopathy
    
    Resource: The Custom Vision resource you created previously
    
    Project Types: Classification
    
    Classification Types: Multiclass (single tag per image)?
    
    Domains: ?
    
4. Click [+] Add images, and select all of the files in the positive image folder you extracted previously. Then upload the image files, specifying the tag positive

5. Repeat the previous step to upload the images in the negative folder with the tag negative

6. In the Custom Vision project, above the images, click Train to train a classification model using the tagged images. Select the Quick Training option, and then wait for the training iteration to complete (this may take a minute or so).

7. When the model iteration has been trained, review the Precision, Recall, and AP performance metrics - these measure the prediction accuracy of the classification model, and should all be high.

## Milestone 2 - Test the model & Generate Custom Vision link

Before publishing this iteration of the model for applications to use, you should test it.

Above the performance metrics, click Quick Test.

View the predictions returned by your model - the probability score should be around 90%

Then, you can close the Quick Test window.

Now you're ready to publish your trained model and use it from a client application!

Click Publish to publish the trained model with the following settings:

    Model name: Diabetic Retinopathy detection 

    Prediction Resource: The prediction resource you created previously.

After publishing, click the Prediction URL icon to see information required to use the published model. Later, you will need the appropriate URL and Prediction-Key values to get a prediction from an Image URL, so keep this dialog box open and carry on to the next task.

## Milestone 3 - Layout of Power App

Go to https://make.powerapps.com and sign in with your organizational account.

The following figure shows the main development window when you enter Power Apps Studio:

image?

detailed process?

The app can run on mobile, install the Power Apps Mobile app on your phone. When building an app, you should test it in the same form factor as your users!

## Milestone 4 - Link Custom Vision model and Power App

text

link

## Milestone 5 - App accuracy test with new inputs

text

link

## Knowledge test

https://docs.microsoft.com/en-us/learn/modules/classify-images-custom-vision/3a-knowledge-check

https://docs.microsoft.com/en-us/learn/modules/get-started-with-powerapps/6-powerapps-quiz-get-started

## Next steps

Learning more about Custom Vision: https://docs.microsoft.com/en-us/learn/paths/explore-computer-vision-microsoft-azure/

Learning more about Canvas App creation:https://docs.microsoft.com/en-us/learn/paths/create-powerapps/

Azure Health bot by using built-in or custom scenarios: https://docs.microsoft.com/en-us/learn/paths/create-bots-azure-health-bot/

AI business school for healthcare: https://docs.microsoft.com/en-us/learn/paths/ai-business-school-healthcare/?WT.mc_id=sitertzn_homepage_mslearn-card-aibusinessschool

The Value of Computer Vision in Healthcare Panel in [this video](https://www.youtube.com/watch?v=dbISoN71rrY)



## Optional Transfer Knowledge activity

You can modify your app to analyze images, including generating a descriptive caption, extracting relevant tags, identifying objects, determining image type and metadata, detecting human faces, known brands, and celebrities, and others. You can find out more about using the Computer Vision service in the [service documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/computer-vision/).

With Power Apps, you can:

Build an app quickly by using the skills that you already have.

Connect to the cloud services and data sources that you're already using.

Share your apps instantly so that coworkers can use them on their phones and tablets.

## Feedback

Be sure to give [feedback about this workshop](https://forms.office.com/r/MdhJWMZthR)!

[Code of Conduct](CODE_OF_CONDUCT.md)

