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

### Rank 0 Tensors:
- 1 is a scalar, has magnitude but no direction, no feature
- 1 can be one cloud, one line 

### Rank 1 Tensors:
- Bike features:

|Brand|Price|Speed|CC|Breaks|Gares|
|---|---|---|---|---|---|
|Honda|75K|120kmph|125|Disk|4|

- Each value in the table represents magnitude of the tensor. 
- Above raw values converted to values using NLP, so as to do math on them.
- In Tensor all the feature of magnitude should be of same type like( Int,Float,string) refereed to as **dtype**
- Rank 1 tensor is a vector
- Rank 1 Tensor has different magnitude with different direction but measuring one direction.
- 6 features = 6 shape = 6 magnitude
- N - dimensions still talking about a tensor so still rank 1 holds good for this tensor.

### Rank 2
- List of rows and columns 
- Matrix combination of vectors. 
- Magnitude and intersection of two directions 
- 3X3 Matrix (11,12,13,21,22,23,31,32,33)
- Rank 0 has one dimension so no moment
- Rank 1 has to move across columns A1,A2 & A3

|A1|A2|A3|
|---|---|---|
|Bike|400$|Gare|
- Rank 2 Travers across two directions A an B
- Position changes and can also depends on previous values. 
- We can create connections between two consecutive tensors and compare their relations.

|XX|A1|A2|A3|
|---|---|---|---|
|B1|A1B1|A2B1|A3B1|
|B2|A1B2|A2B2|A3B3|
|B3|A1B3|A2B3|A3B3|

### Rank 3 
- We have 3 different tensors to measure magnitude.
- We can compare a  phone with has RBG R(3X3),B(3X3),G(3X3)
-  ![Rank3](https://github.com/vurachaitanya/ML_AI/blob/master/Images/Rank%203%20tensor.jpg)
