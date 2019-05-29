---
title: "The Awesome Adventures of Captain Spirit"
author_profile: true
excerpt: "The Awesome Adventures of Captain Spirit⛄is a narrative standalone free game developed by Dontnod Entertainment."
order: 1
header:
  teaser: /assets/images/projects/captainspirit/teaser_captainspirit.jpg
gallery:
  - url: /assets/images/projects/captainspirit/captainspirit1.jpg
    image_path: assets/images/projects/captainspirit/captainspirit1.jpg
  - url: /assets/images/projects/captainspirit/captainspirit2.jpg
    image_path: assets/images/projects/captainspirit/captainspirit2.jpg
  - url: /assets/images/projects/captainspirit/captainspirit3.jpg
    image_path: assets/images/projects/captainspirit/captainspirit3.jpg
  - url: /assets/images/projects/captainspirit/captainspirit4.jpg
    image_path: assets/images/projects/captainspirit/captainspirit4.jpg
  - url: /assets/images/projects/captainspirit/captainspirit5.jpg
    image_path: assets/images/projects/captainspirit/captainspirit5.jpg
  - url: /assets/images/projects/captainspirit/captainspirit6.jpg
    image_path: assets/images/projects/captainspirit/captainspirit6.jpg
---
{: .text-justify}
The Awesome Adventures of Captain Spirit⛄is a narrative standalone free game developed by Dontnod Entertainment. It is available on Steam/Xbox One/Playstation 4. 

You follow Chris Eriksen, a young boy who creates the superhero alter ego Captain Spirit and you uncover the issues he is dealing with.

{% include video id="faWhiRLSsnc" provider="youtube" %}

## What I did on this project

{: .text-justify}
Starting from scratch, I took care of the Motionbuilder pipeline for the animators. My goal was to make tools for the them so they could animate in the best conditions.
Here are some of the tools I've done:

* **Exporter Tool** to export and ensure all animations are compliant with our pipeline by applying metadata such as a production statuses.
* **Reference Tool** (like in [Maya](https://knowledge.autodesk.com/support/maya/learn-explore/caas/CloudHelp/cloudhelp/2018/ENU/Maya-ManagingScenes/files/GUID-238914C9-4129-454C-99D7-B8C57AF423DB-htm.html)), linked to Perforce, to load elements (characters, props...) in the animator's working scene.
* **Sequence Tool** to retrieve UE4 cameras within Motionbuilder.
* **Quick Rig Tool** to quickly generate rigs for animated props.
* **Scene Checker** to make sure everything's fine before exporting the animations.
* **Video Reference Tool** to automatically retrieve video references for the currently edited animations.
{: .text-justify}
I also continued to improve and maintain the existing tools I made during Vampyr and took care of compliance on consoles.

## Documentary

{% include video id="J5jJnA5i6ZA" provider="youtube" %}

## Gallery

{% include gallery %}
