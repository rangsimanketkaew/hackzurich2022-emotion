# hackzurich2022-emotion

ML algorithm for emotion detection for HackZurich 2022 project

## ML model

A pretrained model (`model.h5`) was trained on the FER-2013 dataset, to classify the emotion on a person's face into one of seven categories, using deep convolutional neural networks. The FER-2013 dataset consists of 35887 grayscale, 48x48 sized face images with seven emotions - angry, disgusted, fearful, happy, neutral, sad and surprised.

We trained a model using compute engine on Google cloud provided by Google Zurich.

![alt text](img/hz2022-emotion-results.png "Emotion results")

## Deployment

![alt text](img/hz2022-gce-engine.png)

```sh
gcloud config set project PROJECT_ID
gcloud run deploy
```

![alt text](img/hz2022-deploy.png)
