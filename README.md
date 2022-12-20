# Comparative Analysis on Different Models with HC18 Challenge

#Package dependencies
```
Python 3.9
Pytorch
OpenCV
Tochvision
```

# Data
The data for this challenge can be downloaded from Zenodo, DOI 10.5281/zenodo.1322001 <br>
Saving your data on Google drive with the following format works the best: 
- HC 18
  - data
    - training_set
    - test_set
  - savedModel (which can be added from https://drive.google.com/drive/folders/1DQ6clCjGbcecoBSKLj2N1xBN77FWWCOP?usp=share_link) 

# Masking
Run the Masking.ipynb to transform all masks, you only need to do this step once since it overwrite all annotations

# Dataloader
Feel free to use pre-generated datasets from the pickle files <br>
You can also use Split.ipynb to generate your own datasets

# Models
Run any model you like using the .ipynb files. However, only AttentionUNet++.ipynb and Complete_UNet++.ipynb contain predictions with test dataset <br>
If you don't want to train models, feel free to use pre-trained models from savedModel <br>
You will see dice index for evaluation at the end of each model

# Contributions
Yi contributed Original, Masking, UNet, ResUNet, UNet++, AttentionUNet, AttentionUNet++, and UNet+++ <br>
Bo contributed predictions with test dataset contained in AttentionUNet and UNet++，error analysis with test dataset, loss function modification/analysis, optimizer modification/analysis, Dice loss evaluation modification/analysis.

# Reference
- Thomas L. A. van den Heuvel, Dagmar de Bruijn, Chris L. de Korte and Bram van Ginneken. Automated measurement of fetal head circumference using 2D ultrasound images. PloS one, 13.8 (2018): e0200412.
- Thomas L. A. van den Heuvel, Dagmar de Bruijn, Chris L. de Korte and Bram van Ginneken. Automated measurement of fetal head circumference using 2D ultrasound images [Data set]. Zenodo. http://doi.org/10.5281/zenodo.1322001
- Foivos I. Diakogiannis, Franc ̧ois Waldner, Peter Caccetta, and Chen Wu. Resunet-a: a deep learning framework for semantic segmentation of remotely sensed data. ArXiv cs.CV, 1904(00592), 2019. https://doi.org/10.1016/j.isprsjprs.2020.01.013.
- Kaiming He, Xiangyu Zhang, Shaoqing Ren, and Jian Sun. Deep residual learning for image recognition. ArXiv cs.CV, 1512(03385), 2015. https://doi.org/10.48550/arXiv.1512.03385.
- Chen Li et al. Attention unet++: A nested attention-aware u-net for liver ct image segmentation. 2020 IEEE International Conference on Image Processing (ICIP), 2020. https://doi.org/10.1109/ICIP40778.2020.9190761.
- Ozan Oktay, Jo Schlemper, Loic Le Folgoc, Matthew Lee, et al. Attention u-net: Learning where to look for the pancreas. ArXiv cs.CV, 1804(03999), 2018. https://doi.org/10.48550/arXiv.1804.03999.
- Olaf Ronneberger, Philipp Fischer, and Thomas Brox. U-net: Convolutional networks for biomedical image segmentation. MICCAI, 2015. Springer.
- Zongwei Zhou, Md Mahfuzur Rahman Siddiquee, Nima Tajbakhsh, and Jianming Liang. Unet++: A nested u-net architecture for medical image segmentation. ArXiv cs.CV, 1807(10165), 2018. https://doi.org/10.48550/arXiv.1807.10165.4
