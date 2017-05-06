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

Details on what the heck TensorFlow actually is: https://www.tensorflow.org/get_started/get_started
You can use tensorboard to visualize your graph: https://www.tensorflow.org/get_started/summaries_and_tensorboard

`%qtconsole` executed within a cell gives you a terminal. 

If using an interactive session in tensorflow, don't have to worry about doing sess.run() everywhere, can instead just do <tensor>.eval or <operation>.run without referencing the sess.
