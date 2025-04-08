---
title: Launching the App
---

So we can interact with the dataset, launch the FiftyOne UI. This can also be
done via the Python SDK.

```terminal:input
text: |-
    session = fo.launch_app(dataset, auto=False)
```

Normally if working on a local machine you would access the UI at the URL
`http://localhost:5151`. To access the UI from this workshop session, you can
access the UI at the following URL. Clicking on this will in this case open it
within a tab of this workshop session dashboard.

```dashboard:reload-dashboard
name: FiftyOne
url: {{< param ingress_protocol >}}://fiftyone-{{< param session_hostname >}}{{< param ingress_port_suffix >}}
```
