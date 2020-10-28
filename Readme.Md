Attrition

### S10 Implementing LR
#### 1.	Add CutOut from transformations (albumentations)
#### 2.	Implement LR Finder (for SGD, not for ADAM) Source: https://github.com/davidtvs/pytorch-lr-finder
#### 3.	Implement ReduceLROnPlatea Source: https://pytorch.org/docs/stable/optim.html#torch.optim.lr_scheduler.ReduceLROnPlateau
#### 4.	Find best LR to train your model
#### 5.	Use SDG with Momentum
#### 6.	Train for 50 Epochs.
#### 7.	Show Training and Test Accuracy curves
#### 8.	Target 88% Accuracy.
#### 9.	Run GradCAM on the any 25 misclassified images. Make sure to mention what is the prediction and what was the ground truth label.


### Results:
#### Arranging file structure

-----|models </br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|---  __init.py__ <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|--- *Resnet* Files , resnetbase <br>
------|dataloader.py <br>
------|datamodel.py </br>
------|gradcam.py <br>
------|lrfinder.py  <br>
------|optimizer.py <br>
------|transformation.py <br>

#### 1.	Added Dropout in Albumentation
#### 2.	Implemented LR Finder for SGD taken from Source: https://github.com/davidtvs/pytorch-lr-finder
#### 3.	Implemented ReduceLROnPlatea. Source: https://pytorch.org/docs/stable/optim.html#torch.optim.lr_scheduler.ReduceLROnPlateau
#### 4.	Best Learning Rate - 0.001
#### 5.	Accuracies in Last few epochs ranging Train 97.4%, Test: 88.5%
#### 6. Best Accuracy Train - 97.58%(Epoch 50) Test - 88.83%(Epoch 50)

### Train & Test Acc Curves Twinx
<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/Train%20&%20Test%20Acc%20Curves%20Twinx.png" width="550" title="Twinx">
                                                                                                                                         
### Gradcam Images
<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_0_car.png" width="550" title="car">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_1_truck.png" width="550" title="truck">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_2_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_3_dog.png" width="550" title="dog">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_4_dog.png" width="550" title="dog">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_5_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_6_dog.png" width="550" title="dog">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_7_horse.png" width="550" title="horse">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_8_bird.png" width="550" title="bird">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_9_ship.png" width="550" title="ship">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_10_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_11_plane.png" width="550" title="plane">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_12_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_13_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_14_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_15_frog.png" width="550" title="frog">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_16_bird.png" width="550" title="bird">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_17_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_18_plane.png" width="550" title="plane">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_19_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_20_deer.png" width="550" title="deer">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_21_deer.png" width="550" title="deer">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_22_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_23_cat.png" width="550" title="cat">

<img src="https://github.com/haricharanvihari/extensive_viz/blob/master/S10_DNN/Images/gradcam_incorrect_24_car.png" width="550" title="car">

