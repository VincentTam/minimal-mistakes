---
title: "Life is Strange 2"
author_profile: true
excerpt: "Life is Strange 2 👨‍👦  is a narrative game developed by Dontnod Entertainment."
order: 1000
header:
  teaser: /assets/images/projects/lifeisstrange2/teaser_lis2.jpg
gallery:
  - url: /assets/images/projects/lifeisstrange2/lis21.jpg
    image_path: assets/images/projects/lifeisstrange2/lis21.jpg
  - url: /assets/images/projects/lifeisstrange2/lis22.jpg
    image_path: assets/images/projects/lifeisstrange2/lis22.jpg
  - url: /assets/images/projects/lifeisstrange2/lis23.jpg
    image_path: assets/images/projects/lifeisstrange2/lis23.jpg
  - url: /assets/images/projects/lifeisstrange2/lis24.jpg
    image_path: assets/images/projects/lifeisstrange2/lis24.jpg
  - url: /assets/images/projects/lifeisstrange2/lis25.jpg
    image_path: assets/images/projects/lifeisstrange2/lis25.jpg
  - url: /assets/images/projects/lifeisstrange2/lis26.jpg
    image_path: assets/images/projects/lifeisstrange2/lis26.jpg
---
{: .text-justify}
Life is Strange 2 👨‍👦  is a narrative game developed by Dontnod Entertainment. It is available on Steam/Xbox One/Playstation 4.

You follow the Diaz brothers, Sean and Daniel, on their journey from Seattle, USA to their father's home town of Puerto Lobos, Mexico. 

{% include video id="ma94jdiMFhQ" provider="youtube" %}

## What I did on this project

{: .text-justify}
I continued to improve the animation's pipeline started on [Captain Spirit](https://pgui.github.io/portfolio/captainspirit/#what-i-did-on-this-project), making it more tightly coupled to our data mining system to improve planning and prevent production bottlenecks.

{: .text-justify}
I also pushed further our [Leaflet](https://leafletjs.com/) integration, implementing a database to keep track of qa testers runs on each level of the game for each platform. This way, we could track not only the location of the controlled pawn in-game, but also the performance at each recorded point (frame time, memory...).

{: .text-justify}
Then, the database allows us to query points answering certain criteria and display them on the map (for example: all the points on *Level1* where the frame time was above *35 milliseconds* using *perforce changelist 700000*).

## Gallery

{% include gallery %}
