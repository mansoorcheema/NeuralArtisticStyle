# NeuralArtisticStyle
Implementation of Neural Art Deep Learning paper.(https://arxiv.org/abs/1508.06576).
This very simple and nice algorithm describes the process how we can mix the content of one image with the style of another image to generate new artisitic images (with content coming from our chosen image). Most specifically, using this algorithm we can represent the content of an image as painted by a famous artist like \"Picasso\". This is done by creating a new image via merging the content of one image and style from another image. *I.e.,* $$Content\\ Image+Style\\ Image=Resultant\\ Image$$\n
### Content Image
<img src=\"./golden_gate.jpg\" width=\"200\" caption=\"Conent+\">

### Style Image
<img src=\"./frida_kahlo.jpg\" width=\"200\"> 

### Resultant Image
<img src=\"./golden_gate_kahlo.png\" width=\"200\">

**Transfer Learning** For representing the content and style of given images we will make use of already learned weight of a [deep network](http://arxiv.org/pdf/1409.1556.pdf) (Please read this beautifully written [paper](http://arxiv.org/abs/1508.06576) to get the complete understanding of the algorithm). For this regard, you will download already trained 19-Layers deep neural network (vgg) model and plug cost functions at specific layers of this already trained model and rerun the back-propogation algorithm to learn the merging weights, content and style representation via minimizing a loss function. You can download the learned model from following [link](http://www.vlfeat.org/matconvnet/models/beta16/imagenet-vgg-verydeep-19.mat)\n"
