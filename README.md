# Python-ImageSearch

it's a wrapper around pyautogui and opencv2, to allow you to easily add cross-platform image searching capabilities
to your project.

See the documentation for examples. If you have any questions feel free to contact me.

Documentation : https://brokencode.io/how-to-easily-image-search-with-python/

This is the currently maintained package, so if you've come from
https://pypi.org/project/python-imagesearch-drov0/

you are at the right place

## Easy Example:

## Install:

> pip install python-imagesearch

You may need to install dependencies depending on your OS:

### Linux :
```
sudo pip3 install python3-xlib
sudo apt-get install scrot python3-tk python3-dev python3-opencv
```
### Windows :

No setup should be needed 

### MacOs : 
```
brew install opencv
pip3 install -U pyobjc-core
pip3 install -U pyobjc
```
I have not tested myself as I don't own a mac, but it was tested and documented in this issue : https://github.com/drov0/python-imagesearch/issues/5

## Quick start

The simplest example to do image search with python is this:

```
from python_imagesearch.imagesearch import imagesearch

pos = imagesearch("./github.png")
if pos[0] != -1:
    print("position : ", pos[0], pos[1])
else:
    print("image not found")
```

this searches for one occurrence of the image “github.png” on the screen and print its x/y position 

Some advanced examples exists here (yes I shut down my blog and forgot to save it): https://web.archive.org/web/20221130045749/https://brokencode.io/how-to-easily-image-search-with-python/

Exact function definitions can be found here: https://github.com/drov0/python-imagesearch/blob/master/python_imagesearch/imagesearch.py 
