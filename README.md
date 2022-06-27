# Image-Caption-Generation
Image Captioning: Implementing the Neural Image Caption Generator with python

## Photo and Caption Dataset
Flickr8k_Dataset: Contains 8092 photographs in JPEG format.
Flickr8k_text: Contains a number of files containing different sources of descriptions for the photographs.

The dataset has a pre-defined training dataset (6,000 images), development dataset (1,000 images), and test dataset (1,000 images).

One measure that can be used to evaluate the skill of the model are BLEU scores.

1. BLEU-1: 0.401 to 0.578.
2. BLEU-2: 0.176 to 0.390.
3. BLEU-3: 0.099 to 0.260.
4. BLEU-4: 0.059 to 0.170.

## Requirements
1. Tensorflow
2. Keras
3. Numpy
4. h5py
5. Pandas
6. Pillow
7. Pyttsx

## Develop Deep Learning Model
1. Loading Data.
2. Defining the Model.
3. Fitting the Model.
4. Complete Example.

## Defining the Model

![image](https://user-images.githubusercontent.com/66959193/175902750-14363a3e-907d-4f85-935d-bd7768671937.png)

## Plot of the Caption Generation Deep Learning Model

![image](https://user-images.githubusercontent.com/66959193/175903012-227b9a4e-1da8-4371-b5f5-e7af18f944ec.png)

## Output
The output of the model is a caption to the image.

## Results
Following are a few results obtained after training the model for 70 epochs.

Image | Caption 
--- | --- 
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/beach.jpg" width="400"> | **Generated Caption:** A brown dog is running in the water.
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/image.jpg" width="400"> | **Generated Caption:** A tennis player hitting the ball.
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/child.png" width="400"> | **Generated Caption:** A child in a helmet is riding a bike.
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/street.png" width="400"> | **Generated Caption:** A group of people are walking on a busy street.


On providing an ambiguous image for example a hamsters face morphed on a lion the model got confused but since the data is a bit biased towards dogs hence it captions it as a dog and the reddish pink nose of the hamster is identified as red ball

Image | Caption
--- | ---
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/9.jpg" width="400"> | **Generated Caption:** A black dog is running through the snow with a red ball.


In some cases the classifier got confused and on blurring an image it produced bizzare results

Image | Caption
--- | ---
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/img1.jpg" width="400"> | **Generated Caption:** A brown dog and a brown dog are playing with a ball in the snow.
<img src="https://github.com/Shobhit20/Image-Captioning/blob/master/test/img1_blur.jpg" width="400"> | **Generated Caption:** A little girl in a white shirt is running on the grass.




