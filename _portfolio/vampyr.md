---
title: "Vamp<span style=\"color:red\">**y**</span>r"
author_profile: true
excerpt: "Vampyr🧛is a narrative driven Action-RPG developed by Dontnod Entertainment."
order: 1
tags:
  - dontnod
  - narrative game
  - unreal engine 4
  - xbox one
  - playstation 4
  - pc
  - c++
  - csharp
  - python
  - javascript
  - leaftletjs
  - motionbuilder
  - maya
  - tools
header:
  teaser: /assets/images/projects/vampyr/teaser_vyr.jpg
gallery:
  - url: /assets/images/projects/vampyr/vyr1.jpg
    image_path: assets/images/projects/vampyr/vyr1.jpg
  - url: /assets/images/projects/vampyr/vyr2.jpg
    image_path: assets/images/projects/vampyr/vyr2.jpg
  - url: /assets/images/projects/vampyr/vyr3.jpg
    image_path: assets/images/projects/vampyr/vyr3.jpg
  - url: /assets/images/projects/vampyr/vyr4.jpg
    image_path: assets/images/projects/vampyr/vyr4.jpg
  - url: /assets/images/projects/vampyr/vyr5.jpg
    image_path: assets/images/projects/vampyr/vyr5.jpg
  - url: /assets/images/projects/vampyr/vyr6.jpg
    image_path: assets/images/projects/vampyr/vyr6.jpg
---

Vampyr🧛is a narrative driven Action-RPG developed by Dontnod Entertainment and edited by Focus Home Interactive. It takes place in a 1918 London ravaged by the Spanish influenza; you are a doctor who just came back from the war and unfortunately, you also just turned into a vampire...
{: .text-justify}
Your goal is to find a cure for your condition; for that, you'll meet a wide range of characters across London and you'll be able to eat all of them !
{: .text-justify}
You can find more informations on [the website of the game](http://www.vampyr-game.com/).
{: .text-justify}

Here is a trailer to set the mood

{% include video id="_YLhQJSwCQo" provider="youtube" %}

## What I did on this project

I have the chance to be part of a cross project team, meaning I have to make tools working on all Dontnod's projects made with UE4. I had to extend the editor with new fonctionnalities, creating new features for the proprietary tools and improving pipelines for certain teams. 
These tools are used by a wide range of people, from designers to animators, and they aim to boost their productivity.  
The hardest part is to release new functionalities within a short time range with a very small team.
Here is some notable things I've done:
{: .text-justify}
* **Data Mining** setup. From the automatic data extraction from Unreal to the front-end display in a web page using [DataTable](https://datatables.net/).
* A **Map System** (like google maps) using [LeafletJS](http://leafletjs.com/). Vampyr being an open world, it was very useful for the designers (display items placement, ennemies locations and have an overview of the level design) or the environment artists (to see the work accomplished and which parts of the world still need to be done). On the main lines, it uses commands called periodically by the continuous integration system:
  * Unreal Screenshot command to update the map's visuals.
  * Unreal command to extract the actor's informations (name, location...) to display markers on the map.
  * Feeding all of the above in Leaftlet.
* **Automatic Jira Tasks** from placeholder actors in the levels. Level designers could place placeholder actors in the levels for objects they would need but not available yet. By adding custom metadata, which I implemented, to the object, such as a description or if it is animated or not, it would automatically create a Jira task in the database to be treated by the right team. It uses a mix of Unreal command to extract the actor's placeholder metadata and a python command with some [python Jira](https://jira.readthedocs.io/en/master/) code.
* I also spent a lot of time making **Tools & Pipelines** for the animators by making python tools in Motionbuilder as:
  * A custom animation exporter.
  * Export of the cinematic's cameras and animation's timings from Unreal to Motionbuilder, so that animators can polish only used and visible parts of an animation.  
  * Tool to load objects as references in the animator's working scenes.
  * Perforce integration in Motionbuilder.
{: .text-justify}
Oh yes, I also took care of some parts on the compliance on Playstation 4 and Xbox One, providing me an experience developing on consoles.
{: .text-justify}
## Gallery
{% include gallery %}
