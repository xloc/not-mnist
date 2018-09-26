# Usage

Use the following command to restore the .npz file
```bash
cat not_mnist.npz.part_* > not_mnist.npz
```

# Struture

```python
nm = np.load('not_mnist.npz')
images = nm['images']
# images.shape == (529114, 28, 28)
labels = nm['labels']
# lables.shape == (529114,)
```
