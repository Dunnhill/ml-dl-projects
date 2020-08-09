# Content

*Photographic style transfer is a long-standing problem
that seeks to transfer the style of a reference style photo
onto another input picture.*

This notebook covers four types of style transfer: usual style transfer, mask style transfer, double style transfer, double mask style transfer.
Each type of transfer was performed on several different image-examples.
A more detailed description of each type and a visual example of execution is provided below.

### 1.   Usual style transfer based on the [paper](https://openaccess.thecvf.com/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf) 

*General scheme:* 

> input + content + style = output

<img src='https://s8.hostingkartinok.com/uploads/images/2020/08/f4c319bb8ed83431ec7e9a8396da44c8.png' width=1000/></a>

### 2.   Mask Style Transfer

The image style is applied to the area that corresponds to the white color in the mask image.
> input + content + *mask* + style = output

<img src='https://s8.hostingkartinok.com/uploads/images/2020/07/ab3eefabbc52d87519d90cc4c2217f1c.png' width=1000/></a>

### 3.   Double Style Transfer 

Two image styles are applied to an image at the same time.
> input + content + style-1 + style-2 + mask = output

<img src='https://s8.hostingkartinok.com/uploads/images/2020/08/b0799341d1d192aad8bf2d979acd9e11.png' width=1000/></a>

### 4.   Double Mask Style Transfer 

Two styles are applied to the image based on the input mask.
> input + content + mask + style-1 + style-2  = output

<img src='https://s8.hostingkartinok.com/uploads/images/2020/08/e5007cf210260e7dedf8a35cfbd6f696.png' width=1000/></a>


# Notes

* Used framework: [PyTorch](https://pytorch.org/)

* To focus only on the style of the output image, *the content image* is always selected as *the input image*. If desired, you can use white noise.

* Used CNN: [VGG-19](https://arxiv.org/pdf/1409.1556.pdf) as simple CNN architecture.

* This project was inspired by one seminar of [Deep Learning School](https://www.dlschool.org/) (spring, 2020)

* All calculations was made using [Colaboratory Google (Colab) ](https://colab.research.google.com/)
