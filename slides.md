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

## Outline

1. What is GeoJupyter?
2. Why GeoJupyter?
3. JupyterGIS
4. **Why you should get involved**
5. How you can get involved


## View the slides on the web

![<https://mfisher87.github.io/presentation-cng2025/>](/assets/images/qr.svg)

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

**JupyterGIS** is our flagship project; a GIS platform in JupyterLab that can be used in some similar ways to QGIS.
We'll talk more about JupyterGIS shortly.

But our work is far from limited to JupyterGIS; not everything we build is going to be a
huge project.
It depends on what our community (that's you!) tells us they need.
:::


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* Even experts often struggle
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

* Even experts often struggle
* [Friction when visualizing from a programming environment]{.fade}
* [Linked visualizations are difficult to build]{.fade}
* [Lack of tools for visualizing vertical landscapes]{.fade}
* [Repeatable GIS layouts and symbology]{.fade}


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


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* [~~Even experts often struggle~~]{.fade}
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


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* [~~Even experts often struggle~~]{.fade}
* [~~Friction when visualizing from a programming environment~~]{.fade}
* Linked visualizations are difficult to build
* [Lack of tools for visualizing vertical landscapes]{.fade}
* [Repeatable GIS layouts and symbology]{.fade}


## TODO: Linked visualizations


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* [~~Even experts often struggle~~]{.fade}
* [~~Friction when visualizing from a programming environment~~]{.fade}
* [~~Linked visualizations are difficult to build~~]{.fade}
* Lack of tools for visualizing vertical landscapes
* [Repeatable GIS layouts and symbology]{.fade}

## TODO: Vertical landscapes


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* [~~Even experts often struggle~~]{.fade}
* [~~Friction when visualizing from a programming environment~~]{.fade}
* [~~Linked visualizations are difficult to build~~]{.fade}
* [~~Lack of tools for visualizing vertical landscapes~~]{.fade}
* Repeatable GIS layouts and symbology


## TODO: Repeatable GIS layouts and symbology


## :shrug: Why GeoJupyter?

:face_with_head_bandage: Existing workflows have some painful gaps:

* [~~Even experts often struggle~~]{.fade}
* [~~Friction when visualizing from a programming environment~~]{.fade}
* [~~Linked visualizations are difficult to build~~]{.fade}
* [~~Lack of tools for visualizing vertical landscapes~~]{.fade}
* [~~Repeatable GIS layouts and symbology~~]{.fade}

_And much, much more!!_

:::notes
The landscape of open source geospatial tools is far from perfect.

What we are attempting to bring to the table is a holistic approach to evaluating and
improving this landscape.
To achieve this, we're taking a human-centric approach to finding and addressing these
gaps.
So far we've conducted dozens of hours of user interviews to understand what folks need
most, and we'll continue to use the input of real people to guide our priorities.
:::


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

* :studio_microphone: [Sign up for an interview](https://geojupyter.org/interviews/sign-up)!
* :test_tube: [Try JupyterGIS!](https://jupytergis.readthedocs.io/) Where does it meet your needs? Where does it fall short?
* :memo: [Report bugs, request features!](https://github.com/geojupyter/jupytergis/issues)
* :gift: [Open Pull Requests!](https://github.com/geojupyter/jupytergis)
* :left_speech_bubble: [Chat with us on Zulip!](https://jupyter.zulipchat.com/#narrow/channel/471314-geojupyter)
* :sunglasses: Contribute your awesome vibes to our community!
* :ballot_box: Help develop community governance and scaffolding!
* :moneybag: Fiscal sponsorship!

:::notes
There are lots of avenues for supporting this work.
Reach out to me if you're interested in contributing! 
:::


## View the slides on the web

![<https://mfisher87.github.io/presentation-cng2025/>](/assets/images/qr.svg)


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
