# Self_Supervised_Learning_with_RHEED 

## What is RHEED?
 >RHEED(Reflection High Energy Electrion Diffraction) is one of methodology to  characterize the surface of crystalline materials. RHEED shot the electron beam by its special gun to surface of materials, which makes reflected electrons. These reflected electrons collides with detector and it makes unique pattern depend on the matterials. 

 The patterns have been analysized by numerous of ML like PCA, really classical method to classify the matterial's pattern and understand its property. And we adopted the art-of-state method Self-Supervised Learning method proposed by Google and Meta.
 

## What is Self-Supervised Learning?

> The CNN was a kind of revolution to computer vision area. But it has really critical problems. That is that it is too expensive to create proper dataset and its labeling even a real laboratory doesn't have enough money to classify the data. Because it spend so much time of poor graduate student Google and Meta proposed the algorithms for computer to understand the difference of images and calculate its loss to classify the images by computer even labels for data is not required.

These algorithms was crucial to diagnose the COVID-19. Unlikely the time of graduate student is cheap, time of Doctors are expensive to label thousands X-ray picture. the time of physicist is priceless, we made accepted this algorithms for RHEED.

## What I dedicated to this project?

### 0. Background

This research was supported by Smart Surface Material Lab. in UoS and KRCIT(Korea Research Institute of Chemical Technology). The data was provided by Smart Surface Material Lab and I participated in data analysis parts by self-supervised learning.

The main idea was that our images are really similar to medical images. These are gray-scale, anomaly detection and classification. So, I found a paper, [How Transferable are Self-supervised Features in Medical Image Classification Tasks?](https://arxiv.org/abs/2108.10048)[1]by Bayer in Germany. Following the flow of this paper, we choose models and got a bit clues, how to preprocess the data or how to validate the results.

Unfortunately, I am not so good at solid state physics. Many colleagues help me understand data significance and interpretation. I purposed this project but it was clear that It was impossible to research this area without their help. 


###  1. Data

Data was provided by Smart Surface Lab. 

> 1. More 1,000 pictures.
> 2. Split with Validation, Test, Train. 
> 3. Normalized by Torch likely other medical case analysis in Kaggle
> 4. Under ResNet



 ### 2. Model selection

Based on [1], concerned paperwithcode and its rank of performance.

> 1. MoCo
> 2. SImCLR
> 3. SwAV
> 4. BYOL

### 3. Embedding

By Lightly, generated the embedded space and observed its tendency.
Colleagues who is engaged in solid state physics advised. They give me some feedback then, edited some hyper-parameters or preprocessing. 

## Other references and links
 Data_from_Dropbox
>https://www.dropbox.com/sh/jszs15w46dlwa6i/AACiRn7A4FwUkMsN2Ax_Q7M_a?dl=0

 Kaggles

>1. https://www.kaggle.com/code/yasufuminakama/ranzcr-resnext50-32x4d-starter-training
>2. https://www.kaggle.com/code/shivanandmn/self-supervise-momentum-contrast-great-idea/notebook?scriptVersionId=54013004
>3. https://www.kaggle.com/code/ayuraj/v2-self-supervised-pretraining-with-swav/notebook?scriptVersionId=60346393

 Models
>1. https://paperswithcode.com/sota/self-supervised-image-classification-on?tag_filter=25

Lightly( Zurich )
> 1. https://github.com/lightly-ai/lightly
