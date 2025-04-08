---
title: Workshop Summary
---

This was a quick example showing how one could integrate FiftyOne with Educates
to create a workshop.

The workshop has been structured so that it can be hosted in Educates running
in Kubernetes, or you could run it locally in a Docker environment if you have
the `educates` CLI by running:

```workshop:copy
text: educates docker workshop deploy -f https://github.com/GrahamDumpleton/lab-fiftyone-testing/releases/latest/download/workshop.yaml
```

and then subsequently deleting it by running:

```workshop:copy
text: educates docker workshop delete -f https://github.com/GrahamDumpleton/lab-fiftyone-testing/releases/latest/download/workshop.yaml
```
