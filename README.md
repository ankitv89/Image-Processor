# Human body measurement

Human body measurement is a image processing software use in identify body parts, calculate body measurements.

  - Take your picture in one color background
  - Enter your height and choose input image path
  - Magic!!!

### Version
0.0.1

### Tech

Human body measurement uses a number of open source projects to work properly:

* The Python Standard Library
* NumPy - The fundamental package for scientific computing with Python
* Scikit-image - Image processing in Python

### Installation

### Todo's

* Familiar with scikit-image library, numpy, matplotlib
  * Scikit-image modules: data, io, feature, filter
  * Numpy: numpy-array, operators
  * Matplotlib: show image, plot, axes
* Remove noise in input image (front image, side image)
  * Read image as grayscale image
  * Apply Kuwahara - Nagao filter
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
