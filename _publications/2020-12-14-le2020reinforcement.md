---
title: "Reinforcement learning-based optimal complete water-blasting for autonomous ship hull corrosion cleaning system"
authors: "Anh Vu Le, Phone Thiha Kyaw, Prabakaran Veerajagadheswar, MA Viraj J Muthugala, Mohan Rajesh Elara, Madhu Kumar, Nguyen Huu Khanh Nhan"
collection: publications
permalink: /publications/2020-12-14-le2020reinforcement
date: 2020-12-14
venue: "Ocean Engineering"
year: 2020
pdfurl: 'https://www.sciencedirect.com/science/article/pii/S0029801820313846?casa_token=b8486kAbdewAAAAA:jE9gwqyA-tKqw0TBA3QHwyvxhKz2vOGq2V9PkVh98_Rj1WJ3IpfUm_V3yNk6tBqOlPusjsOErWTuDg'
classes: wide
share: false
---

## Abstract

Routine cleaning of the corroded ship hulls in dry dock maintenance guarantees the smooth operation of the shipping industry. Deploying the autonomous system to remove the corrosion by water-blasting is a feasible approach to ease the burden in manual operation and to reduce water, time, and energy consumption. In this paper, the water-blasting framework is proposed for a novel robot platform named Hornbill with the adhesion mechanism by permanent magnetic, self-localization by sensor fusion to navigate smoothly on a vertical surface. Hence, we propose a complete waypoint path planning (CWPP) to re-blast the self-synthesizing deep convolutional neural network (DCNN) based corrosion heatmap by initial-blasting. The optimal CWPP problem, including the shortest travel distance and shortest travel time to save water, power while ensuring visiting all predefined waypoints by benchmarking output, is modeled as the classic Travel Salesman Problem (TSP). Further, the Pareto-optimal trajectory for given TSP has been driven by the reinforcement learning (RL) technique with a proposed reward function based on the robot's operation during blasting. From the experimental results at the shipyard site, the proposed RL-based CWPP generates the Pareto-optimal trajectory that enables the water-blasting robot to spend about 10% of energy and 9% of water less than the second-best evolutionary-based optimization method in various workspaces.
{: .text-justify}

{% highlight bibtex %}
@article{le2020reinforcement,
  title={Reinforcement learning-based optimal complete water-blasting for autonomous ship hull corrosion cleaning system},
  author={Le, Anh Vu and Kyaw, Phone Thiha and Veerajagadheswar, Prabakaran and Muthugala, MA Viraj J and Elara, Mohan Rajesh and Kumar, Madhu and Nhan, Nguyen Huu Khanh},
  journal={Ocean Engineering},
  pages={108477},
  year={2020},
  publisher={Elsevier}
}
{% endhighlight %}