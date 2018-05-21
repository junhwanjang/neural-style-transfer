# Style Transfer with Convolutional Neural Network

A tensorflow implementation of style transfer (neural style) described in the papers:
* [A Neural Algorithm of Artistic Style](https://arxiv.org/pdf/1508.06576v2.pdf) : *submitted version*
* [Image Style Transfer Using Convolutional Neural Networks](http://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf) : *published version*  
by Leon A. Gatys, Alexander S. Ecker, Matthias Bethge

## Results
- Original Image
![](https://github.com/junhwanjang/neural-style-transfer/blob/master/images/cat.png)
- Style Image
![](https://github.com/junhwanjang/neural-style-transfer/blob/master/images/style_cow.png)
- Output Image
![](https://github.com/junhwanjang/neural-style-transfer/blob/master/results/cat_1013.jpg)

## Usage

### Prerequisites
1. Tensorflow
2. Python packages : numpy, scipy, PIL(or Pillow), matplotlib
3. Pretrained VGG19 file : [imagenet-vgg-verydeep-19.mat](http://www.vlfeat.org/matconvnet/models/imagenet-vgg-verydeep-19.mat)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;* Please download the file from link above.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;* Save the file under `model`

### Running
```
python run_main.py --content <content file> --style <style file> --output <output file>
```
*Example*:
`python run_main.py --content images/cat.png --style images/style_cow.png --output result.jpg`


