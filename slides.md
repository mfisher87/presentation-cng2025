---
title: "🌐 GeoJupyter 🌐<br/>@<br/>🌥️ CNG '25 🌥️"
subtitle: |
  TODO
title-slide-attributes:
  data-notes: |
    Hi! I'm used to presenting remotely, so I hope you'll forgive my nervousness today.
format: "revealjs"
---

## Outline

1. What is GeoJupyter?
2. Why GeoJupyter?
3. JupyterGIS
4. **Why you should get involved**
5. How you can get involved


## :wave: Hi, I'm Matt!

:::evenly-spaced
:computer: Research Software Engineer (RSE)

:people_holding_hands: Community Engagement Manager

:seedling: Working at Schmidt DSE @ UC Berkeley

:snowflake: Previously at National Snow & Ice Data Center (NSIDC)

:open_hands: Open source maintainer: [earthaccess](https://github.com/nsidc/earthaccess), [viscm](https://github.com/matplotlib/viscm), several conda-forge feedstocks
:::

:::notes
I'm Matt Fisher, and I'm a Research Software Engineer and Community Engagement
Manager for GeoJupyter.

Before GeoJupyter, I worked in building software for research support and data
analysis, visualization, management, and access at the National Snow and Ice Data
Center.

I'm a maintainer of several open source projects.
Maybe we've spoken on GitHub before!
_earthaccess_ is another community-owned project I help maintain, one of my favorites.
It enables access to NASA data in 3 lines of code;
a huge improvement: before _earthaccess_ you had to write >100 lines to authenticate and
interact with the NASA earth science data API.
:::


{{< include lets-chat.md >}}

:::notes
I have lots of stuff I want to talk to you all about!
I hope we can find each other later and chat :)

Also, if you want to check out these slides and follow the links, they are publicly
available online.

I'm not going to go through this slide now; I'll show it again at the end, so don't
worry if you didn't catch the URL.
:::


## In this talk...

::::::columns
:::{.column width=50%}
* What is GeoJupyter?
* Why GeoJupyter?
* What is JupyterGIS?
* How you can join the community
:::

:::{.column width=50%}
![[mfisher87.github.io/presentation-cng2025/](https://mfisher87.github.io/presentation-cng2025/)](/assets/images/qr.svg){width=100%}
:::
::::::

:::notes
In this talk, I'm going to introduce the GeoJupyter community and discuss why it exists.
I'll then introduce and demo the JupyterGIS software.
Finally, we'll talk about how you can join the community.

These slides are available on the web at this URL, as well as on GitHub.
If you missed it, don't worry, I'll leave this slide up at the end.
:::


## :question: What is GeoJupyter?

<br />
<br />

:::elevator-pitch
<hr />

GeoJupyter is an open and community-driven effort to [reimagine geospatial interactive
computing experiences]{.jupyter-orange} to enable **more people to
confidently engage with geospatial data**.

<hr />
:::

:::notes
_Read the slide_
:::

## Our values

<br />

:cartwheeling: **Approachability** and **playfulness**, like desktop GIS tools

<br />

:feather: **Flexibility** and **reproducibility**, like coding methods

<br />

:performing_arts: **Collaboration** and **storytelling**, like Jupyter Notebooks


## :people_holding_hands: It's a communtity!

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
:::{.column width=60%}
:abacus: Do some analysis

:floppy_disk: Write out a data file

:inbox_tray: Download it to local machine

:world_map: Open QGIS, load basemap, load data file

:eyes: Validate, inspect, explore

:shower: Repeat
:::

:::{.column width=40%}
![](/assets/images/gis-bounce-hard.jpg)
:::
::::::


<!-- alex ignore easy -->
## :woman_dancing: _The GIS Bounce_ :man_dancing: (easy mode)

::::::columns
:::{.column width=60%}
:abacus: Do some data analysis

:snake: Write one line of code!

(Imports don't count :smirk:)

```python
from jupytergis import explore

explore(my_geodataframe)
```

:eyes: Validate, inspect, explore

:shower: Repeat
:::

:::{.column width=40%}
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
* :test_tube: [Try JupyterGIS](https://jupytergis.readthedocs.io/)! Where does it meet your needs? Where does it fall short?
* :gift: [Report bugs, request features](https://github.com/geojupyter/jupytergis/issues)!
  [Open Pull Requests](https://github.com/geojupyter/jupytergis)!
* :left_speech_bubble: [Chat with us on Zulip](https://jupyter.zulipchat.com/#narrow/channel/471314-geojupyter)!
* :sunglasses: Contribute your rad vibes to our community!
* :compass: Become a community leader!
* :moneybag: Fiscal sponsorship!

:::notes
There are lots of avenues for supporting this work.
Reach out to me if you're interested in contributing!
:::


# :tada: Bonus slides

{{< include lets-chat.md >}}
