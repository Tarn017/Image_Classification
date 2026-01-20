# Image_Classification

**1.** To start, download the following file and drop it in the folder you are working in: 

**2.** After that, create a new python file in that same directory. Copy the following code into that file:
```python
from train_NN import CNN

if __name__ == "__main__":
```
**Important:** Everything you do from now on should be inserted below the code you just copied. It's also important to 

**Example**
```python
from train_NN import CNN

if __name__ == "__main__":
    CNN(
        train_path="./klass_daten/",
        epochs=30,
        lr=0.005,
        conv_filters=[16, 32, 64, 128],
        fully_layers=[256],
        resize=(128, 128),
        model_name='peter',
        train_split=0.9,
        droprate=0.5,
        augmentation=[0.1,0.1,0.1,0.1,0.1],
        dec_lr=10e-5
    )
```
