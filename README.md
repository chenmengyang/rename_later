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

## GOAL
* Rebuild the [original deeplab](https://github.com/tensorflow/models/tree/master/research/deeplab) using tensorflow [Estimator](https://www.tensorflow.org/guide/estimators)
* Features
  * Train
  * Evaluation (Show miou for each classes)
  * Tensorboard (Visulise prediction results in real time)

## PLAN & TODOLIST


## References

1.  **Rethinking Atrous Convolution for Semantic Image Segmentation**<br />
    Liang-Chieh Chen, George Papandreou, Florian Schroff, Hartwig Adam.<br />
    [[link]](http://arxiv.org/abs/1706.05587). arXiv: 1706.05587, 2017.

2.  **Encoder-Decoder with Atrous Separable Convolution for Semantic Image Segmentation**<br />
    Liang-Chieh Chen, Yukun Zhu, George Papandreou, Florian Schroff, Hartwig Adam.<br />
    [[link]](https://arxiv.org/abs/1802.02611). In ECCV, 2018.
