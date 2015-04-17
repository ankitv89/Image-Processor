# Human body measurement

Human body measurement is a image processing software use in identify body parts, calculate body measurements.

  - Take your picture in one color background
  - Enter your height and choose input image path
  - Magic!!!

### Version
0.0.1

### Tech

Human body measurement uses a number of open source projects to work properly:

* NumPy - The fundamental package for scientific computing with Python
* Scikit-image - Image processing in Python

Test and view tools

* IPython
* IPython notebook

### Installation

* Python: sudo apt-get install python-pip python-dev build-essential
* Dependencies: pandas, sympy, nose. (pip install 'lib-name')
* Numpy: sudo pip install numpy
* Matplotlib: sudo pip install matplotlib
* Scipy: sudo pip install scipy
* Tool (ipython, ipython notebook): pip install ipython, pip install "ipython[notebook]"
* Scikit-image: pip install -U scikit-image
* How to use ipython-notebook: https://www.youtube.com/watch?v=H6dLGQw9yFQ

### Procedure For Image Capture
* Lighting: Bright environment with as much natural light as possible
* Background: Removal of obstructions with a single color background
* Border: Encapsulate entire body in the center of image
* Clothing: Underwear
* Pose - Front - Feet: Shoulder width apart
* Pose - Front - Arms: Facing the floor at a 45 degree angle
* Pose - Front - Hands: Flat with length of wrists facing the camera
* Pose - Side - Arms: Flat against body not obstructing front or back outline
* Pose - Side - Hands: Flat with width of wrists facing the camera

### Steps For Processing Image
#### Filter Input (all steps)
To minimize errors, **only necessary** information should be used. The challenge of having too little or too much information helps to minimize errors. An added benefit of filtering large datasets is reduced computation requirements for processing.
* Remove noise
* Narrow field to region of interest

#### Extract Features & Information (one or a combination of all)
* *Color information* - looking for changes in color or detect objects.
* *Blob extraction* - detecting adjacent, similarly colored pixels.
* *Edges and corners* - examining changes in brightness to identify borders or objects.
* *Pattern recognition and template matching* - adding basic intelligence by matching features with the features of known objects.

### Todo's

* Familiar with scikit-image library, numpy, matplotlib
  * Scikit-image modules: data, io, feature, filter
  * Numpy: numpy-array, operators
  * Matplotlib: show image, plot, axes
* Remove noise in input image (front image, side image)
  * Read image as grayscale image
  * [Remove salt and pepper noise](http://scikit-image.org/docs/stable/auto_examples/plot_nonlocal_means.html#example-plot-nonlocal-means-py)
* Remove background of image
  * Finding edges of human in image by roberts (canny / sobel) fitler
  * [Skin detection](http://www.codeproject.com/Articles/38176/Image-Processing-Skin-Detection-Some-Filters-and-E)
  * Merge regions to find the human in image (skimage.segmentation.*)
* Body parts recognition 
  * Using skeletonization method to get structure of human body 
  * Compare with human body region to get the body parts
  * Label each body parts
* Calculate the measurements of body parts
  * Calculate the body parts by draw eclipse

### Documents
https://drive.google.com/drive/u/0/folders/0B7rKJ3215ikuOU4xTzZPWm9FVU0

License
----

© 2015 - Boopis Media.
