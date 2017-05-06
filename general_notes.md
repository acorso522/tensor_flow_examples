
# Installing zshell

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### If using Agnoster theme
```shell
git clone https://github.com/powerline/fonts
cd fonts
./install.sh from terminal / command line
Open iTerm2->Preferences->Profiles->Change Font-> 12pt Meslo LG S DZ Regular for Powerline
```



# Install TensorFlow

Install pip and virtualenv

```shell
sudo easy_install pip
sudo pip install --upgrade virtualenv
```

Create a virtualenv in a new directory

```shell
virtualenv --system-site-packages ~/tensorflow
```
--system-site-packages brings in all other site packages

Activate the environment

```shell
source ~/tensorflow/bin/activate
```

Now, install TensorFlow just as you would for a regular Pip installation. First select the correct binary to install and then pip install.

```shell
export TF_BINARY_URL=https://storage.googleapis.com/tensorflow/mac/gpu/tensorflow-0.10.0-py2-none-any.whl
pip install --upgrade $TF_BINARY_URL
```
a
To deactivate the virtualenv 

```shell 
(tensorflow)$ deactivate
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





