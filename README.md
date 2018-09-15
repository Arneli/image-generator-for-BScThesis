parametric-face-image-generator(extension by arneli00)
==========================================================

This software is based on the parametric-face-image-generator of the gravis group. The [original Software](https://github.com/unibas-gravis/parametric-face-image-generator) enables you to generate fully parametric face images from the Basel Face Model 2017 as proposed in:

- [1] Adam Kortylewski, Andreas Schneider, Thomas Gerig, Bernhard Egger, Andreas Morel-Forster and Thomas Vetter 
["Training Deep Face Recognition Systems with Synthetic Data"](https://arxiv.org/abs/1802.05891), 
IN: arXiv preprint (2018)


- [2] Adam Kortylewski, Bernhard Egger, Andreas Schneider, Thomas Gerig, Andreas Morel-Forster and Thomas Vetter 
["Empirically Analyzing the Effect of Dataset Biases on Deep Face Recognition Systems"](https://arxiv.org/abs/1712.01619), 
IN: arXiv preprint (2017)

You can control the variation of parameters such as pose, shape, color, camera and illumination based on your demand and application.
This dataset can be used for training and comparing machine learning techniques such as CNNs on a common ground as proposed in [1] by generating fully controlled training and test data.

WHAT'S NEW
----------
This version produces two images of the same face at a time. For the first image, it uses the Basel Face Model "face12" and for the other image the "bfm" version. This version only works for three occlusionModes. These are:

### random
This mode renders an arbitrary image of a hand or a microphone over the output image

### random-1
This mode renders an image of a hand over the image

### random-2
This mode renders an image of a microphone over the image

### box
This mode occludes the image with a rectangle at a random position, with random shape and random color

### none
If you don't want an occlusion to be added to the image, specify this option


OUTPUT
------
This modified version provides two new folders in the output (in this version, the output is split in two: output/bfm and output/face12):

### img_masks
These images provide the ground truth segmentation of the image. It distinguishes between face-region, occlusion-region, and background.

### img_occlusion
The original images overlaid with an occlusion of one of the above modes.


Contributors
------------

- Bernhard Egger
- Adam Kortylewski
- Andreas Morel-Forster
- Andreas Schneider

Maintainers
-----------

- University of Basel, Graphics and Vision research: [@unibas-gravis](https://github.com/unibas-gravis), [homepage](http://gravis.cs.unibas.ch)


License
-------

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0), details see LICENSE

    Copyright 2017, University of Basel, Graphics and Vision Research

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

