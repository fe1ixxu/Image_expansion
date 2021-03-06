# Image expansion with GANs
In this project, we are presenting a deep learning approach for adversarially training
neural networks to naturally expend image boundaries. We use a three-phase training schedule to
stably train a DCGAN architecture on a subset of the Places365 dataset. Once trained, our model
is able to expend 128 × 128 color images relatively realistically, thus allowing for recursive
expansion.

## Install Requirement

```
sudo apt-get install curl
conda install --yes --file requirements.txt
```
## Get Started

### Download and prepare data:

```
chmod +x ./prepare_data.sh
./prepare_data.sh
```
dataset looks like:

<div align=center>
<img src="https://github.com/fe1ixxu/Image_expansion/blob/master/images/data.png" alt="PAPR" width="512px">
</div>

### Training the model:

```
python image_expansion_main.py
```

## Test and see results:
```
python image_expansion_test.py
```
<div align=center>
<img src="https://github.com/fe1ixxu/Image_expansion/blob/master/images/result.png" alt="PAPR" width="512px">
<img src="https://github.com/fe1ixxu/Image_expansion/blob/master/images/result2.png" alt="PAPR" width="512px">
</div>

## Built With

* [Keras](https://www.tensorflow.org/guide/keras)
* [TensorFlow](https://www.tensorflow.org)
* [OpenCV](https://opencv.org)
