### Requirments.txt
- tensorflow==2.4.1
- tensorflow-datasets==4.1.0
- Pillow==8.1.0
- numpy
- pandas
- matplotlib

#### Import required modules :
`!pip install tensorflow tensorflow-datasets Pillow numpy pandas matplotlib `


```
import tensorflow as tf
import tensorflow_datasets as tfds
print(tfds.__version__)
from PIL import Image
print(Image.__version__)
import numpy as np
import urllib3
import pandas as pd
import matplotlib.pyplot as plt
```

### Tensor 
- A Mathematical representation for the magnitudes of a collection of features.
- N dimensional Array
- Container for holding data
- Represents a set of magnitudes of components
- N different Axes
- Components are features for ML.

#### Rank 0 Tensors:
- 1 is a scalar, has magnitude but no direction, no feature
- 1 can be one cloud, one line 

#### Rank 1 Tensors:
- 
