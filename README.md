## Medical image  caption generation with VGG160-LSTM and Vission transformer-GPT2
This dataset includes around 530 images along with 5 different captions written by different people for each image.
The images are all contained together while caption text file has captions along with the image number appended to it. The zip file is approximately over 1 GB in size.
![image](https://github.com/user-attachments/assets/a472763a-3b18-4acf-876e-fbfa30a437df)


Viewing similar images
When the VGG-16 model finishes extracting features from all the images from the dataset, similar images from the clusters are displayed together 
to see if the VGG-16 model has extracted the features 
correctly and we are able to see them together.
![image](https://github.com/user-attachments/assets/12bb7074-e62c-46c7-9aff-0976927cdeb1)


Link the text and image data(model fusion=VGG16-LSTM)
In this dataset, a single image has 2-10 captions. I will only use one caption out of 5 for simplicity.
Each row of the dtexts and dimages contain the same info. Remove captions (or images) that do not have corresponding images (or captions).
![image](https://github.com/user-attachments/assets/e0288917-37e9-42d7-b04a-4d665c50faa9)


These generated captions are compared to the actual captions from the dataset and evaluated using BLEU scores as the evaluation metrics. 
A score closer to 1 indicates that the predicted and actual captions are very similar. As the scores are calculated for the whole test data, 
we get a mean value which includes good and not so good captions. Some of the examples can be seen below:
![image](https://github.com/user-attachments/assets/43792bbd-4d66-4eed-8550-5ea417d4fabd)

![image](https://github.com/user-attachments/assets/f8fcc4b7-97b0-40ed-89aa-43e3625cc187)
