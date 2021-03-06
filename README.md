# imageCaptioningAndAudio
Generate Captions and Audio for the respective image

## What the project is?

In this project if you give an input image,our code will generate the corrosponding caption(natural language description) for the respective image and also you will hear a speech which describes the respective image.
Hence This will be very helpful for visually impared persons to know what is present in an image by listening to the audio which describes what the image is about!

## Features and concepts used

We have used encoders and decoders in this  project,the encoder is CNN(resnet-152,pretrained on ILSVRC-2012-CLS image classification dataset) while the decoder used is LSTM

We have used nltk for the preprocessing task,argparse to accept command line arguments,etc.
The entire code is implemented in pytorch as the deep learning library.



## Examples

<img src="https://github.com/pranav-msc/imageCaptioningAndAudio/blob/main/ex.jpg" width="300" height="300"> 
Caption generated for the corrosponding image-
a man wearing a suit and tie with a tie .


We also have other samples images on which you can read the corrosponding caption and hear the respective caption.


## How to run the code

1.Very first stp is to clone this repo

2.[Link to download pretrianed model file(save these files inside models directory)](https://www.dropbox.com/s/ne0ixz5d58ccbbz/pretrained_model.zip?dl=0)


After downloading the pretrained weights the only thing need to be done is to test the model

run the command to generate and hear the text(on terminal)-

3.python3 sample.py --image "path of the image"


example code   -   ``` python3 sample.py --image ex.jpg ```

## Note

It might be possible that you may see by some errors(in case of error running sample.py)-

So make sure you install requirements.txt file if you are popped by an error related to importing of a file,using these commands you can also download the dataset,so you may skip last 2 lines if you don't want to download dataset


```
pip install -r requirements.txt
chmod +x download.sh
./download.sh
```

And also make sure you have libraries like gtts and its other sub modules or functions installed



In case the problem is not resolvable contact us!


## Reference


[Click here to go the reference link](https://github.com/yunjey/pytorch-tutorial/tree/master/tutorials/03-advanced/image_captioning)


## Project Members:


Pranav Kotgire


Ravi Chopra


Deependra yadav

