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
      83fn0608.jpg
      ...
  ```
  The filename(99ak0449) is the label.
  
* Refer to ```parameters.py``` and begin training by ```python training.py```.
