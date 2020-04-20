<!-- This file is automatically generated by tfds.scripts.document_datasets and
all modifications will be erased, please edit the original document_datasets.py
file. -->
# Datasets

Note: The datasets documented here are from `HEAD` and so not all are available
in the current `tensorflow-datasets` package. They are all accessible in our
nightly package `tfds-nightly`.

---

## `##` starts a line comment for mako, so we have to come up with following
## trick to output double '#' for markdown. Same for backslashes.
${"##"} Usage

```python
# Build the `tf.data.Dataset` pipeline.
ds, info = tfds.load('cifar10', split='train', shuffle_files=True, with_info=True)
ds = ds.shuffle(info.splits['train'].num_examples)
ds = ds.batch(32)

# `tfds.as_numpy` converts `tf.Tensor` -> `np.array`
for ex in tfds.as_numpy(ds):
  # `int2str` returns the human readable label ('dog', 'car',...)
  print(info.features['label'].int2str(ex['label']))
```

## `##` starts a line comment for mako, so we have to come up with following
## trick to output double '#' for markdown. Same for backslashes.
${'##'} All Datasets

{toc}

---