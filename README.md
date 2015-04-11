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

### Todo's

* Familiar with scikit-image library, numpy, matplotlib
  * Scikit-image modules: data, io, feature, filter
  * Numpy: numpy-array, operators
  * Matplotlib: show image, plot, axes
* Remove noise in input image (front image, side image)
  * Read image as grayscale image
  * Apply Kuwahara - Nagao filter
    * Caculate the means μi and variances of all the neighbourhoods
    * The pixel is replaced with the μi of the region with the lowest variances
    * Apply two above step through [generic_filter](http://docs.scipy.org/doc/scipy/reference/generated/scipy.ndimage.filters.generic_filter.html)
* Remove background of image
  * Finding edges of human in image
  * Sub image to remove one color background
* Body parts recognition 
  * Using skeletonization method to get structure of human body 
  * Compare with human body region to get the body parts
  * Label each body parts
* Calculate the measurements of body parts
  * Calculate the body parts by draw eclipse

License
----

© 2015 - Boopis Media.
