---
title: Using the Python SDK
---

We will make use of `fiftyone` directly from the Python interpreter, which since
we are using `uv` is started by running:

```terminal:execute
command: uv run python
```

Within the Python interpreter, import the `fiftyone` package.

```terminal:input
text: |-
    import fiftyone as fo
    
```

We need to load a dataset to work on, so also load the FiftyOne Zoo sub package
which provides APIs for download various datasets. Import the `quickstart`
dataset.

```terminal:input
text: |-
    import fiftyone.zoo as foz
    dataset = foz.load_zoo_dataset("quickstart", persistent=True)
    fo.list_datasets()
```

To verify the contents of the dataset, print out details of the dataset.

```terminal:input
text: |-
    print("Just the dataset")
    print(dataset)

    print("\ndataset.schema")
    print(dataset.schema)

    print("\ndataset.stats()")
    dataset.stats(include_media=True, compressed=True)
```
