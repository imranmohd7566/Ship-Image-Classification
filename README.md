# Ship-Image-Classification

A Kaggle dataset of images of 5 difeerent categories of ship images with its labels in a csv file.
I ahve built 2 models for image classification:

  1. Custom model using 6 Conv2D layers, MaxPool2D, followed by flattening and then adding a dropout before dense layer with softmax activation at the end.
     
  2. A model using the MobileNetV2 with 2 Conv2D, MaxPool2D layers followed by flattening and dropout of 0.6 with softmax activation at the end.
     
  Adam optimizer is used in both with a learning rate of 1e-4.
  
As we can see from the results that in the second model the validation accuracy became consistent from 5th epoch but in the custom model the validation accuracy looks to be still improving till 15th epoch as well. So, maybe the custom model can also give us some good results with some extra epochs and some tuning on the learning rate of the optimizer.
  
![image](https://user-images.githubusercontent.com/50734928/188995138-dd87a964-1679-43d8-9d50-bd845e85073f.png)
![image](https://user-images.githubusercontent.com/50734928/188995228-9ddd8a99-9305-4a96-af42-086f0a82cbd0.png)

The resulst on the test dataset can clearly prove that the MobileNetV2 is outperforming the custom model.

Results:

![image](https://user-images.githubusercontent.com/50734928/188995424-571057ba-41f3-4ac4-8f5b-28f1b7d929af.png)
![image](https://user-images.githubusercontent.com/50734928/188995466-02f515df-3c08-450b-a78b-7ef654a73f46.png)
