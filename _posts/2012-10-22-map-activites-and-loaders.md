---
layout: default
published: false
---

# MapActivity, Robolectric and the Loader framework

## Getting started

First we have a class defined as:
```
@ContentView(R.layout.activity_map_view)
public class MapViewActivity extends RoboMapActivity {
...
}
```

We need to wire up a Loader, that contains a custom Observer, which tells the Loader it needs to update its data. Then, when the LoadManager calls deliverResults the data will be available to it.

Glossary (needs revising):

## Loaders

> Loaders as simple, self-contained objects that (1) load data on a separate thread, and (2) monitor the underlying data source for updates, re-querying when changes are detected. This is more than enough to get you through the contents of this post. All Loaders are assumed to be 100% correctly implemented in this post.
