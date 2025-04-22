---
title: "🌐 GeoJupyter 🌐<br/>@<br/>☁️ CNG '25 ☁️"
subtitle: |
  TODO
title-slide-attributes:
  data-notes: |
    Hi, I'm Matt Fisher, and I'm a Research Software Engineer and Community Engagement
    Manager for GeoJupyter.
format: "revealjs"
---

## Outline {.scrollable}

### What is GeoJupyter?

1. ~~Values~~
2. ~~Objectives~~
3. ~~Gaps in the existing ecosystem~~
    a. ~~Visualization (GIS Bounce)~~
    b. ~~Linked visualization~~
    c. ~~Vertical landscapes visualization~~
    d. ~~Saving, repeating, and sharing layouts &amp; symbology~~


### What is JupyterGIS?
1. ~~What makes it unique?~~
2. ?
3. ~~Demo~~


### Why you should get involved

### How you can get involved

1. Put JupyterGIS in front of more users
2. Contribute your needs and experiences
3. Contribute code
4. Contribute vibes


## QR code self-link

TODO

:::notes
If you missed it, don't worry, we'll leave the QR code up at the end.
:::


## :question: What is GeoJupyter? {.smaller}

<br />

:::elevator-pitch
<hr />

GeoJupyter is an open and community-driven effort to [reimagine geospatial interactive
computing experiences]{.jupyter-orange} for education, research, and industry.

We aim to combine the **approachability** and **playfulness** of desktop GIS tools, the
**flexibility** and **reproducibility** of coding-driven GIS methods, and the **collaborative** and
**storytelling** power of Jupyter to enable more researchers, educators, and learners to
confidently engage with geospatial data.

<hr />
:::

:::notes
:::


## :people_holding_hands: A communtity!

![GeoJupyter is **not** software; it's a **community** which will build many things!](/assets/images/venn-diagram.svg)

:::notes
A common point of confusion is the name GeoJupyter vs JupyterGIS.
**GeoJupyter** is a community; our interest includes but **is not limited to** GIS.
**JupyterGIS** is a GIS platform in JupyterLab that can be used in some similar ways to QGIS.
We'll talk more about JupyterGIS shortly.
:::


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* Friction when visualizing from a programming environment
* Linked visualizations are difficult to build
* Lack of tools for visualizing vertical landscapes
* Repeatable GIS layouts and symbology

:::notes
These are only a few examples we've heard from geospatial practitioners;
we're not actively solving all of these problems right now, but we might give it a try eventually!
:::


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* Friction when visualizing from a programming environment
* [Linked visualizations are difficult to build]{.fade}
* [Lack of tools for visualizing vertical landscapes]{.fade}
* [Repeatable GIS layouts and symbology]{.fade}


## :woman_dancing: _The GIS Bounce_ :man_dancing: (hard mode)

::::::columns
:::{.column width=50%}
* Do some analysis
* Write out a data file
* Download it to local machine
* Open QGIS, load basemap, load data file
* Validate, inspect, explore
* :shower: Repeat
:::

:::{.column width=50%}
![](/assets/images/gis-bounce-hard.jpg)
:::
::::::


## :woman_dancing: _The GIS Bounce_ :man_dancing: (easy mode)

::::::columns
:::{.column width=50%}
One line of code! (excluding imports :smirk:)

```python
from jupytergis import explore

explore(my_geodataframe)
```
:::

:::{.column width=50%}
![](/assets/images/gis-bounce-easy.jpg)
:::
::::::


## TODO: Linked visualizations

## TODO: Vertical landscapes

## TODO: Repeatable GIS layouts and symbology

# JupyterGIS

:bangbang: Early development :bangbang:

:::notes
The _GeoJupyter_ flagship project...
:::


## What is it? How is it different?

:::incremental
* Interactive GIS environment
* JupyterLab-native (try it in a JupyterHub!)
* Python API
* Supports QGIS project files
* **_Real-time collaboration!_**
:::


## Demo

* GIS environment features: layers, identify, time slider
* Collab features: Nick assist?
* :woman_dancing: _The GIS Bounce_ :man_dancing: in JGIS


## How you can help

* :test_tube: Try JupyterGIS! Where does it meet your needs? Where does it fall short?
* :memo: Report bugs, request features!
* :gift: Open Pull Requests!
* :ballot_box: Help develop and operate community governance and scaffolding!
* :sunglasses: Contribute awesome vibes to our community!


## QR code self-link

TODO


# :tada: Bonus slides

## :handshake: I want to talk to you! {.smaller}

### :left_speech_bubble: Ask me about...

* :people_holding_hands: Community engagement stuff
* :open_hands: Open source stuff
* :muscle: Accessibility stuff
* :package: New Python project/environment management tools (`uv`, `pixi`)


### :ear: I want to ask you about...

* :point_up: All that stuff up there
* :coffee: JavaScript map engines & cloud-native data support
* :hole: What gaps or friction you see in the open source geospatial ecosystem
* :stop_sign: What's stopping your team from integrating JupyterGIS in your workflows


## Brianna's story

[_When our community burned, where was the satellite information?_](https://www.linkedin.com/pulse/when-our-community-burned-where-satellite-information-pag%C3%A1n-phd-8rxwf/?trackingId=goJI9VniOZAI3RGuoPXysA%3D%3D)

::::::columns
:::{.column width=25%}
![](/assets/images/brianna-pagan.jpg)
:::

:::{.column width=75%}
> ...we are failing the people and causes that need us the most.
:::
::::::

-- Brianna Pagán, Technical Program Lead @ Development Seed, ex-NASA Deputy DAAC Manager

:::notes
> I should be able to do this. I have a PhD in Remote Sensing, I have built satellite data
> processing pipelines, I help manage one of the NASA satellite data centers, I teach
> courses on climate resilience, adaptation and geoinformatics. […] and yet the irony is
> that with all my experience I could not access the information I knew existed to help
> our community.

End-quote. You can read Brianna's full story by following the link at the top of the slide.
:::
