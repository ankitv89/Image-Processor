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
  * Head part: head, neck
  * Torso
  * Two wirsts, two legs
* Calculate the measurements of body parts
  * Shoulder
  * Neck
  * Chest
  * Waist 

License
----

© 2015 - Boopis Media.
