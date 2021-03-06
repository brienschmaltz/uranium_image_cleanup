# Uranium Image Cleanup
--------

This package was developed to process grayscale uranium images in a specified directory to remove text/labels.

You should already have installed Python 2.7 - 4.0 with PIP. Python will need to be added as an environment variable.

On Window's start Command Prompt or PowerShell. On Linux open up a terminal. 

## To install:
```
    >>> pip install uranium-image-cleanup
```

## Run on Windows:
Type "uic".
```
    >>> uic
    >>>
    >>> *** Uranium Image Cleanup  ***
    >>> Enter Image/s Retrieval Directory:
```

## How to find the uic.exe on Windows:
In case you wanted to move it to the desktop for easy access. 
```
    >>> where uic
    #Output: C:\Users\your_username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.       9_qbz5n2kfra8p0\LocalCache\local-packages\Python39\Scripts\uic.exe
    >>>
```

## Alternative way of running:
On Window's start Command Prompt or PowerShell. On Linux open up a terminal. 

Run python.

```
    >>> python
```

Import the package then call main.

```
    >>> import uic_package as uic
    >>> 
    >>> uic.main()
    >>>
    >>> *** Uranium Image Cleanup  ***
    >>> Enter Image/s Retrieval Directory:
```

## This package is also capable of:

- Removing text/noise on a single image of uranium.
- Detecting white pixels on a single image.

Below are examples on how to implement these.

###### Remove labels on a single image:

``` 
    >>> import uranium_image_cleanup_package as uic
    >>> import opencv as cv2
    >>>
    >>> image uranium_nucleus_10593520                  
    >>> result_image = uic.removeLabel(uranium_nucleus_10593520)

```
###### Detect white pixels on a single image:
``` 
    >>> import uranium_image_cleanup_package as uic
    >>> import opencv as cv2
    >>>
    >>> image uranium_nucleus_10593520                  
    >>> white_pixel_image = uic.detectWhite(img)
```

For more info and access to all the methods available, consult the removeLabel.py script found in the uic_package folder.

----------------------------



