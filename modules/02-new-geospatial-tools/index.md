---
title: "📚 Materials"
---

:::{note} Objectives
* Introduce the GeoJupyter community.
* Introduce LeafMap & JupyterGIS.
* Explore new capabilities of JupyterGIS.
:::


## Presentation

<iframe
  src="https://docs.google.com/presentation/d/e/2PACX-1vRb5KS2we1ql4K1gzLXOdzzfEzD9LmYdSZFQNg5hExbTYWapGYoDkHmcyyTlZqglSdBXBeMT-hmf7zf/pubembed?start=false&loop=false&delayms=60000"
  frameborder="0" width="960" height="569" allowfullscreen="true"
  mozallowfullscreen="true" webkitallowfullscreen="true">
</iframe>

[Direct link](https://docs.google.com/presentation/d/16PppU0B-D-_HmcdLbgsjHX_r7FhmM3Y9B-14uGrj3e4/edit?usp=sharing)


## Introduction to [GeoJupyter](https://geojupyter.org/)

[GeoJupyter](https://geojupyter.org/) is a community, **not** software.

:::{figure} https://raw.githubusercontent.com/mfisher87/presentation-cng2025/b2c31dfc0d5552059c82ee4d75cdb6f2faee4f3f/assets/images/venn-diagram.svg
:label: GeoJupyterCommunityDiagram
:alt: GeoJupyter community diagram
:height: 300px
:align: center

A diagram of the GeoJupyter community's current and future projects.
:::

Our mission is to **enable more people to confidently engage with geospatial data**.

To do this, we're asking people about the way they work and how it makes them feel.
Where are they frustrated? Where are they rewarded?
We allow this input to guide our strategy instead of attempting to guess what to work
on.


### Our values

🤗 **Open source**!

👤 **Human-centered design**!

🤸 **Approachability** and **playfulness**, like desktop GIS tools

🪶 **Flexibility** and **reproducibility**, like coding

🎭 **Collaboration** and **storytelling**, like Jupyter Notebooks


### How to be a part of our community and mission

📅 [**View or save our community calendar**](https://geojupyter.org/calendar) -
Join a hackathon or community meeting!

🗨️ [**Chat with us on Zulip**](https://jupyter.zulipchat.com/#narrow/channel/471314-geojupyter) -
Ask questions or share ideas!

🎤 [**Sign up for an interview**](https://geojupyter.org/interviews/sign-up.html) -
Tell us where you experience friction, frustration, joy, and/or payoff!


## Introduction to [JupyterGIS](https://jupytergis.readthedocs.io/en/latest/)

[JupyterGIS](https://jupytergis.readthedocs.io/en/latest/) is the GeoJupyter community's flagship project.
It is a **collaborative** GIS tool **built in to JupyterLab**.

:::{important}
**JupyterGIS is in early development!**
You may encounter rough edges or bugs.

❤️ We would be thrilled to hear about your experience!
Please let us know about it by [opening a new issue on our GitHub repository](https://github.com/geojupyter/jupytergis/issues/new/choose).
:::

It features its own project file format, `.jGIS`, but also has limited support for QGIS
`.qgz` project files!

It can do many of the same things that QGIS can do:
Manage many map layers,
configure symbology,
and identify features or grid cells.

It also has some capabilities out-of-the-box that QGIS doesn't have:
Google-Docs-like collaborative editing and comments (we call them "Annotations"),
a layer browser with many cloud-native layers pre-populated,
and seamless Jupyter Notebook integration.
Soon, JupyterGIS will also have a STAC browser!


### Streamlined data validation

One of the most common sources of friction reported by practitioners in GeoJupyter
interviews was repeatedly switching between a Notebook environment and a point-and-click
GIS environment (like QGIS and ArcGIS) to check their work.

These practitioners described a process with many steps, like a dance. We heard this so
often, we gave it a name:
["The GIS Bounce"](https://geojupyter.org/blog/20250410-community-insight-gis-bounce/).

We recently released a new feature which streamlines this process.
Now, you can pass your data to JupyterGIS' point-and-click GIS environment with
**one line of code**.

```python
from jupytergis import explore

explore(my_geodataframe)
```

:::{figure} ../../assets/images/jgis-explorer.jpg
:label: JupyterGISExplorer
:alt: Using the `explore()` function in JupyterGIS to interactively explore data.

An example of exploring a GeoDataFrame with **one line of code**.
:::
