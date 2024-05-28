# Introduction

:::{note}
You are viewing a working draft with expected completion in early 2025.
:::

Welcome to the book that takes you through the entire workflow of building medical imaging AI models in Python. This book does not focus on specific tasks such as segmentation or registration, but instead attempts to give you the tools to more generally accomplish any medical imaging AI task.

There is a large programming component to this book, as you will learn how to use the nitrain framework to accomplish your medical imaging AI goals. Nitrain builds on top of popular libraries such as pytorch or keras to give you high-level tools specifically aimed at training models on medical imaging datasets.

## In this book

Each chapter of this book can be read independently, so if you are looking to enhance your skills in one specific area then feel free to skip around. The book is generally organized according to the various steps of a medical imaging AI workflow.

We begin in `1. Handling images` by showing how to read medical images into memory and perform a variety of core tasks such as visualization, operations, and basic processing. Once you've grasped how to work with medical images individually, you will learn in `2. Loading datasets` how to represent entire collections of images and associated metadata in nitrain. We will show you how to specify all kinds of structures that will eventually be fed into your model, including multi-image inputs or outputs.

In `3. Generating batches`, we demonstrate how you can combine images together into trainable units called tensors. Here, you will learn about applying data augmentation to get more out of your data. You will also learn about samplers - a really cool feature of nitrain that simplifies the process of training on slices, patches, or blocks of images.

We move forward to `4. Creating models`, where you will learn how to take advantage of architectures in nitrain to quickly create popular types of models. We will talk about how to use pre-trained models from the community or how to create your own model in pytorch or keras.

The fun part begins in `5. Training models` when you get to put everything together to train models locally, in the cloud, or on the nitrain.dev platform. You'll learn how to ensure that training goes smoothly, or at least how to know when it doesn't.

A unique feature of medical imaging is that reoccuring, or fixed, parts of the images have meaning. That's why in `6. Explaining results` you will learn how to apply various algorithms that can probe your trained model to better understand the image parts to which your model pays closest attention.

Finally, in `7. Sharing and deploying` we wrap up by showing you how to make your model available for others to fine-tune or to use for prediction on new data. We give some advice on how to publish your models as well.

All in all, this book takes you through the entire workflow of reading in medical images to explaining and sharing a trained model.

## About nitrain

You may be wondering why we use nitrain to teach you about medical imaging AI workflows. The simple answer is that nitrain is the easiest way to train medical imaging AI models using pytorch or keras. It provides a very clear set of classes that help users easily conceptualize the entire medical imaging AI workflow.

### Similar frameworks

Nitrain is not the only framework that makes it easier to train AI models on medical imaging datasets. Others include ANTsPyNet, Nobrainer, MONAI, Huggingface, and Pytorch Lightning - all fantastic frameworks. However, nitrain provides some features that others dont:

- ability to train and manage models in the cloud directly from the console
- sharing of models with the commmunity and easy fine-tuning of pre-trained models
- algorithms to help you explain model weights in the context of your medical images

While most of the frameworks above provide at least one of these features, none of them provide all like nitrain does. And regardless, there can never be enough good tools for the growing field of medical imaging AI.

## Receiving help

If you have questions about the book specifically, you can post an issue at github.com/nitrain/book. The source code for the book is publically available at that repository. If you have questions about nitrain, you can post an issue at github.com/nitrain/nitrain.

## About the author

Nicholas Cullen has a BS in Systems Engineering from University of Florida and a PhD in Neuroscience from Lund University in Sweden. He has 10+ years of experience developing tools for medical imaging in Python, R, and C++. He has published 40+ high-impact journal articles on biomarkers, clinical trials, and neurodegenerative diseases and has an H-index of 29.

He started nitrain to make medical imaging AI more accessible to non-imaging experts. If you have any questions, he can be reached at nickcullen31@gmail.com.
