# Image-Classification
CIFAR-10 Photo Classification
# CIFAR-10_Dataset_Classfication
---
CIFAR-10 Photo Classification Dataset
CIFAR is an acronym that stands for the Canadian Institute For Advanced Research and the CIFAR-10 dataset was developed along with the CIFAR-100 dataset by researchers at the CIFAR institute.

The dataset is comprised of 60,000 32×32 pixel color photographs of objects from 10 classes, such as frogs, birds, cats, ships, etc. The class labels and their standard associated integer values are listed below.

0: airplane<br>
1: automobile<br>
2: bird<br>
3: cat<br>
4: deer<br>
5: dog<br>
6: frog<br>
7: horse<br>
8: ship<br>
9: truck<br>
---
---
<br><br>
#Model Summary<br><br>
![image](https://user-images.githubusercontent.com/37467941/148189987-7efe98f8-f9fe-4a2c-967a-fd9194c3b5ff.png)<br>



<b>Result<br><br></b>
![image](https://user-images.githubusercontent.com/37467941/148190125-2390fc9f-35c1-4c55-9281-15f96947e9e6.png)<br>
![image](https://user-images.githubusercontent.com/37467941/148193297-e33ed127-3019-466b-8362-6ff78686ab05.png)


---
<br>
## <b>Saving the entire mode<br></b>
from tensorflow.keras.callbacks import ModelCheckpoint  <br>
checkpoint_path='/content/model_checkpoints'<br>
checkpoint=ModelCheckpoint(filepath=checkpoint_path,frequency='epoch',save_weights_only=False,verbose=2)<br>
<b>to delete model</b> --> del model<br>
from tensorflow.keras.models import load_model<br>
model=load_model(checkpoint_path)<br>
<b>manual save</b> --> model.save('my_model') or model.save('my_model.h5')<br>
---
