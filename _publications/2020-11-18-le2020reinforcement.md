---
title: "Reinforcement Learning-Based Energy-Aware Area Coverage for Reconfigurable hRombo Tiling Robot"
authors: "Anh Vu Le, Rizuwana Parween, Phone Thiha Kyaw, Rajesh Elara Mohan, Tran Hoang Quang Minh, Charan Satya Chandra Sairam Borusu"
collection: publications
permalink: /publications/2020-11-18-le2020reinforcement
date: 2020-11-18
venue: "IEEE Access"
year: 2020
pdfurl: 'https://ieeexplore.ieee.org/iel7/6287639/8948470/09262896.pdf'
classes: wide
share: false
---

## Abstract

Applying the automation in covering the areas entirely eases manual jobs in various domestic fields such as site investigation, search, rescue, security, cleaning, and maintenance. A self-reconfigurable robot with adjustable dimensions is a viable answer to improve the coverage percentage for predefined map areas. However, the shape-shifting of this robot class also adds to the complexity of locomotion components and the need for an optimal complete coverage strategy for this new type of robot. The typical complete coverage route, including the least times of shape-shifting, the shortest navigation route, and the minimum travel time, is presented in the article. By splitting the map into the sub-areas similar to the self-reconfigurable robot's available shapes, the robot can design the ideal tileset and optimal navigation strategies to cover the workspace. To this end, we propose a Complete Tileset Energy-Aware Coverage Path Planning (CTPP) framework for a tiling self-reconfigurable robot named hRombo with four rhombus-shaped modules. The robot can reconfigure its base structure into seven distinct forms by activating the servo motors to drive the three robot hinges connecting robot modules. The problem of optimal path planning assisting the proposed hRombo robot to clear optimally all predefined tiles within the arbitrary workspace is considered a classic Travel Salesman Problem (TSP), and this TSP is solved by the reinforcement learning (RL) approach. The RL's reward function and action space are based on robot kinematic and the required energies, including transformation, translation, and orientation actions, to move the robot inside the workspace. The CTPP for the hRombo robot is validated with conventional complete coverage methods in simulation and real workspace conditions. The results showed that the CTPP is suitable for producing Pareto plans that enable robots to navigate from source to target in different workspaces with the least consumed energy and time among considered methods.
{: .text-justify}

{% highlight bibtex %}
@article{le2020reinforcement,
  title={Reinforcement Learning-Based Energy-Aware Area Coverage for Reconfigurable hRombo Tiling Robot},
  author={Le, Anh Vu and Parween, Rizuwana and Kyaw, Phone Thiha and Mohan, Rajesh Elara and Minh, Tran Hoang Quang and Borusu, Charan Satya Chandra Sairam},
  journal={IEEE Access},
  volume={8},
  pages={209750--209761},
  year={2020},
  publisher={IEEE}
}
{% endhighlight %}