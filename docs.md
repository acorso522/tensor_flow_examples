# Python + Tensor Flow


## Setup
If you don't already have it, install Anaconda, which is just an open-source data-science platform. This will include a large number of the pakcages we will use, including `jupyter` which is where we will work on code. We will use Python 3 unless problem present themselves, though tensor flow should be fine with it.

https://www.continuum.io/downloads#macos

This may take a while so give it some time. 


Add the following line to your `.zshrc` file. Need to add the anaconda distribution to your PATH so your computer knows where to look for global commands like `jupyter`. Note that this command will prepend it to the front of your path so you will now use the anaconda distribution by default when running `python` in the command line. 

```shell
export PATH=/Users/AndrewOrso/anaconda3/bin:$PATH
```


## Python + Package setup

Open up a jupyter notebook inside of the directory you want to work in. 

### Install TensorFlow

Install pip and virtualenv

Now, install TensorFlow just as you would for a regular Pip installation.

```shell
pip install tensorflow
```

Run a simple python script to test it out

```python
import tensorflow as tf
hello = tf.constant('Hello, TensorFlow!')
sess = tf.Session()
print(sess.run(hello))
```



# Point Intellij Project Towards Virtualenv

- Go to project structure File drop down
- Add a new Python SDK pointing towards your local virtualenv
- http://stackoverflow.com/questions/20877106/using-intellijidea-within-an-existing-virtualenv


# Installing Keras after installing tensorflow

- Tensorflow is the backend of keras
- http://www.pyimagesearch.com/2016/11/14/installing-keras-with-tensorflow-backend/

# Get working directory and change
```python
import os
cwd = os.getcwd()
cwd
os.chdir('/Users/aorso/Documents/All Projects/RedML/Anomaly Detection/Alex Python Version/alex_liang_anomaly_detection')
os.getcwd()
```

When running import, python will look in the sys.path and so you need to make sure that the module you want is in one of those directories. May or may not include the current working directory.





