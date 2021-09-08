---
layout: page
title: V2X-Sim
description: The First Public Large-scale Collaborative Perception Dataset 
img: /assets/img/Cars-Intersections.PNG
importance: 1
category: NYU Research
---

 V2X-Sim, short for vehicle-to-everything simulation, is the first synthetic collaborative perception dataset in autonomous driving developed by AI4CE Lab at NYU and MediaBrain Group at SJTU to facilitate collaborative perception between multiple vehicles and roadside infrastructure. We collect data from both roadside and vehicles when they are presented near the same intersection. With information from both the roadside infrastructure and vehicles, the dataset aims to encourage research on collaborative perception tasks.

Although not collected from the real world, we use highly realistic traffic simulation software to ensure the representativeness of our dataset compared to real-world driving scenarios. To be more exact, the traffic flow of our recording files is managed by CARLA-SUMO co-simulation, and we currently use three town maps from CARLA to increase the diversity of our dataset. 

I functioned as an undergrad research assistant in this project and worked closely with [Yiming Li](https://scholar.google.com/citations?hl=en&user=i_aajNoAAAAJ), who is the project lead and a PhD student at NYU Tandon. 

Check out the website that I developed [here](https://ai4ce.github.io/V2X-Sim/) for more information and video demo. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/overview.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/cars-1.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/infra-1.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    On the left, an example of collaborative perception. Middle, front cameras of four vehicles in a scene. Right, cameras of infrastructure in a scene.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/SensorSetupNew.PNG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Sensor set up and configuration for both vehicles and infrastructure.
</div>

More information on sensors and data format can be found at the [official website](https://ai4ce.github.io/V2X-Sim/about.html) of our dataset. 
