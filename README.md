# How to restore

Use the following command to restore the .npz file
```bash
cat not_mnist.npz.part_* > not_mnist.npz
# OR
cat not_mnist_eqsize.npz.part_* > not_mnist_eqsize.npz
```

# Struture and Usage

```python
nm = np.load('not_mnist.npz')
images = nm['images']
# images.shape == (529114, 28, 28)
labels = nm['labels']
# lables.shape == (529114,)

ne = np.load('not_mnist_eqsize.npz')
images = ne['images']
# images.shape == (70000, 28, 28)
labels = ne['labels']
# labels.shape == (70000,)
```
