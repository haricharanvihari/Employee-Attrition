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
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/a.png" width="550" title="Twinx">
                                                                                                                                         
### Gradcam Images
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/b.png" width="550" title="car">

<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/c.PNG" width="550" title="car">
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/d.PNG" width="550" title="car">
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/e.PNG" width="550" title="car">
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/f.PNG" width="550" title="car">
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/g.PNG" width="550" title="car">
<img src="https://github.com/haricharanvihari/Employee-Attrition/blob/main/Images/h.png" width="550" title="car">
