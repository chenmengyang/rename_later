# Deeplabv3+

## Model architecture
![deeplabv3+](https://github.com/chenmengyang/rename_later/blob/master/images/deeplab.png?raw=true)
* Encoder
  * DCNN, backbone of the network, can be resnet, xception and mobilenet.
  * ASPP (Atrous Spatial Pyramid Pooling), for improving performances for multi scales inputs.
* Decoder
  * bilinearity upsampling
  * concat with early layers parameter, convs
  * bilinearity upsampling again recover to the input resolution


## PLAN & TODOLIST
