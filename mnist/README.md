The dataset was created as follows in Octave:

```matlab
examples = struct('testX', testX, 'testY', testY, 'trainX', trainX, 'trainY', trainY);
save -6 mnist.mat examples
```

Read dataset in Python

```python
import scipy.io as sio

d = sio.loadmat("mnist.mat")
v = d["examples"][0, 0]

print v['trainX']
```

