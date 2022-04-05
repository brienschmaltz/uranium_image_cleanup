# Uranium Image Cleanup
--------

 This program was designed to take in user input (a directory where images of uranium are stored), ask for an output folder and then proceed to process images in specified directory to remove text/noise only from specific grayscale uranium images.

***Note:*** This program was designed to run much like an executable. We have provided use cases outside of the program running as an exectuable where user input is required.

This tutorial assumes you have already installed the latest Python and have added it to your environmental path. Python will ask you for this when you install it. Check that box. 

Below is an example of how our ideal user should use install and use this package (AFIT = ideal user).

On Window's start Command Prompt or PowerShell. On Linux open up a terminal. 

## To install:

```
    >>> pip install uranium-image-cleanup
```

## Run program using console script on Window's:


```
    >>> where uic
    #Output: C:\Users\your_username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.       9_qbz5n2kfra8p0\LocalCache\local-packages\Python39\Scripts\uic.exe
    >>>
    #Then add location to a python3 command
    >>> python3 C:\Users\your_username\AppData\Local\Packages\PythonSoftwareFoundation.Python.3.9_qbz5n2kfra8p0\LocalCache\local-packages\Python39\Scripts\uic.exe
    >>>
    #Program will start
    >>> *** Uranium Image Cleanup  ***
    >>> Enter Image/s Retrieval Directory:
```

```
    >>> python3 -m uic
    >>> 
    >>> *** Uranium Image Cleanup  ***
    >>> Enter Image/s Retrieval Directory:
```

## Alternative way of running:

On Window's start Command Prompt or PowerShell. On Linux open up a terminal. 

Run python.

```
    >>> python
```

Import the package then call main().

```
    >>> import uranium_image_cleanup_package as uic
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

For more info and access to all the methods available, consult the remove_label.py script.

----------------------------



