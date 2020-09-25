# Tensorflow neural style transfer explained
Neural style transfer is a deep learning technique that allows you to transfer the style of one image onto another, keeping the content of the latter. It is in many respects different from a typical computer vision task: the middle layers of a pretrained model are needed, instead of the last or last but one layer; the input image is updated during training, rather than the model weights; the optimization process occurs on a bounded space (the RGB values of pixels are bounded between 0 and 1) rather than on infinite space for the model weights. These are all conceptually simple ideas that are trickly to implement, which make it a great learning experience to code up neural style network yourself.

The official [Tensorflow neural style transfer tutorial](https://www.tensorflow.org/tutorials/generative/style_transfer) is a great resource for learning neural style transfer, but unfortunately packs too much information in a single tutorial, making it very difficult to digest. It also contains too many convenient tricks that are not essential for completing the task, which distracts the reader from understanding the gist of neural style transfer.

In this Colab, I rewrote the official tutorial, removing unnecessary tricks and explaining the purpose of each part. If you're new to Tensorflow 2 or to neural style transfer, you can start with my Colab to learn the key implementation, then compare it to the official tutorial to see the improvements that the tricks bring.
