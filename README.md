CRNN 

original paper [arxiv](https://arxiv.org/abs/1507.05717).
The CRNN model can be seen as following:
![](https://raw.githubusercontent.com/yunlongdong/CRNN-Keras/master/photo/Network.jpg)

|       File         |Description                                       |
|--------------------|--------------------------------------------------|
|Model .py           |Network using CNN (VGG) + Bidirectional LSTM      |
|Model_GRU. py       |Network using CNN (VGG) + Bidirectional GRU       |
|Image_Generator. py |Image batch generator for training                |
|parameter. py       |Parameters used in CRNN                           |
|training. py        |CRNN training                                     |
|Prediction. py      |CRNN prediction                                   |

## Training
* First download the korean license plate data from [here](https://www.jianguoyun.com/p/DcvAwI8Qq5nBBximlNoB)
* Put the images in ```DB/train``` like following:
  ```
  DB/
    train/
      99ak0449.jpg
      99wj0971.jpg
      ...
  ```
  The filename(99wj0971) is the label. The image can be seen by:
  
  ![](https://raw.githubusercontent.com/yunlongdong/CRNN-Keras/master/photo/99wj0971.jpg)
  
* Refer to ```parameters.py``` and begin training by ```python training.py```.

## Results
* See ```Prediction.py``` for prediction on images.
* Some result can be seen by:
  
  ![](https://raw.githubusercontent.com/yunlongdong/CRNN-Keras/master/photo/result.jpg)
