# AutoDRIVE Simulator HMI
Human Machine Interfaces to AutoDRIVE Simulator

![Framework](Media/Framework.jpg)

This repository uses [AutoDRIVE Ecosystem](https://autodrive-ecosystem.github.io/) to realize an immersive digital twin framework for exploring human-autonomy coexistence. The source repository for AutoDRIVE Ecosystem can be found [here](https://github.com/Tinker-Twins/AutoDRIVE).

## Human Machine Interfaces

<table>
<thead>
  <tr>
    <th align="center"><img src="Media/Keyboard.gif"></th>
    <th align="center"><img src="Media/Mouse.gif"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">Keyboard + Single Monitor Setup</td>
    <td align="center">Mouse + Single Monitor Setup</td>
  </tr>
  <tr>
    <td align="center"><img src="Media/Gamepad.gif"></td>
    <td align="center"><img src="Media/Driving Rig.gif"></td>
  </tr>
  <tr>
    <td align="center">Gamepad + Single Monitor Setup</td>
    <td align="center">Driving Rig + Triple Monitor Setup</td>
  </tr>
</tbody>
</table>

**Observation Interfaces:**
- Single Monitor
- Triple Monitor
- XR Headset

**Interaction Interfaces:**
- Keyboard
- Mouse/Trackpad
- Gamepad
- Driving Rig

In terms of observability, users can choose between different cameras, which allow first-, second-, and third-person viewing. These viewpoints can either be statically rendered on a single/triple-monitor display or dynamically rendered within a mixed-reality framework, which allows for a fully immersive user experience. For interaction, the input methods are mapped across varying scales and configurations of vehicles to allow intuitive control for user convenience. A detailed video highlighting various human-machine interfaces (HMIs) to observe and interact with the autonomy-oriented digital twins in AutoDRIVE Simulator is available on [YouTube](https://youtu.be/_cwrw1w5d_g?feature=shared).

## User Study

We administered the immersive presence of 16 users within the virtual environment of the proposed framework using the Bob G. Witmer Presence Questionnaire (PQ) [[25]](https://doi.org/10.1162/105474698565686), [[26]](https://doi.org/10.1162/105474605323384654). The questionnaire is made available as [Presence Questionnaire.xlsx](User%20Study/Presence%20Questionnaire.xlsx) and the user demographics are recorded in [Demographics.xlsx](User%20Study/Demographics.xlsx). Individual user responses for various observation and interaction interfaces are stored as `CSV` files within the [`User Study`](User%20Study) directory and are post-processed using the [data_analysis.mlx](User%20Study/data_analysis.mlx) script. Following are the post-processed user experience analyses for observation and interaction interfaces:

**Observation Interfaces:**
![User experience analyses for observation interfaces](User%20Study/data_analysis_observation.png)

**Interaction Interfaces:**
![User experience analyses for observation interfaces](User%20Study/data_analysis_interaction.png)

## Case Study

<table>
<thead>
  <tr>
    <th align="center"><img src="Media/Case Study - Physical Twin.gif"></th>
    <th align="center"><img src="Media/Case Study - RViz.gif"></th>
    <th align="center"><img src="Media/Case Study - Digital Twin.gif"></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td align="center">Physical Twin</td>
    <td align="center">State Estimation</td>
    <td align="center">Digital Twin</td>
  </tr>
</tbody>
</table>

In order to evaluate the serviceability of the proposed framework, an edge-case urban driving scenario was devised. The scenario was laid out to jump-scare the ego vehicle and analyze its reactive response to the event. Particularly, the ego vehicle was supposed to keep driving straight unless it was unsafe/unethical to do so (e.g. dead end, traffic sign, traffic light, imminent collision, etc.). Down the road, a semiautonomous virtual vehicle was set up to cut across the ego vehicle as it approached the first 4-way intersection, requiring the ego vehicle to execute a panic-breaking maneuver while ensuring safety in case of any failures.

The individual runs for distinct modes of operation (AV, CAV, HV-S, and HV-D) are stored within the [`Case Study`](Case%20Study) directory and are post-processed using the [data_analysis.mlx](Case%20Study/data_analysis.mlx) script. The following plot depicts the ego vehicle behavior in autonomous (AV), connected autonomous (CAV), human-operated with static HMD (HV-S), and human-operated with dynamic HMD (HV-D) modes of operation:

![Ego vehicle behavior for panic-breaking case study](/Case%20Study/data_analysis.png)

 A time-synchronized video highlighting the case-study is available on [YouTube](https://youtu.be/gYeeRgntkpA?feature=shared).

## Citation

We encourage you to read and cite the following papers if you use any part of this dataset for your research:

#### [Metaverse for Safer Roadways: An Immersive Digital Twin Framework for Exploring Human-Autonomy Coexistence in Urban Transportation Systems](https://arxiv.org/abs/2406.05465)
```bibtex
@inproceedings{Metaverse-for-Safer-Roadways-2024,
author={Samak, Tanmay V. and Samak, Chinmay V. and Krovi, Venkat N.},
booktitle={2024 IEEE Conference on Telepresence}, 
title={Metaverse for Safer Roadways: An Immersive Digital Twin Framework for Exploring Human-Autonomy Coexistence in Urban Transportation Systems}, 
year={2024},
volume={},
number={},
pages={160-165},
doi={10.1109/Telepresence63209.2024.10841549}
}
```
This work has been published in **2024 IEEE Conference on Telepresence (TELE).** The publication can be found on [IEEE Xplore](https://doi.org/10.1109/Telepresence63209.2024.10841549).

#### [AutoDRIVE: A Comprehensive, Flexible and Integrated Digital Twin Ecosystem for Enhancing Autonomous Driving Research and Education](https://arxiv.org/abs/2212.05241)
```bibtex
@article{AutoDRIVE-Ecosystem-2023,
author = {Samak, Tanmay and Samak, Chinmay and Kandhasamy, Sivanathan and Krovi, Venkat and Xie, Ming},
title = {AutoDRIVE: A Comprehensive, Flexible and Integrated Digital Twin Ecosystem for Autonomous Driving Research & Education},
journal = {Robotics},
volume = {12},
year = {2023},
number = {3},
article-number = {77},
url = {https://www.mdpi.com/2218-6581/12/3/77},
issn = {2218-6581},
doi = {10.3390/robotics12030077}
}
```
This work has been published in **MDPI Robotics.** The open-access publication can be found on [MDPI](https://doi.org/10.3390/robotics12030077).

#### [AutoDRIVE Simulator: A Simulator for Scaled Autonomous Vehicle Research and Education](https://arxiv.org/abs/2103.10030)
```bibtex
@inproceedings{AutoDRIVE-Simulator-2021,
author = {Samak, Tanmay Vilas and Samak, Chinmay Vilas and Xie, Ming},
title = {AutoDRIVE Simulator: A Simulator for Scaled Autonomous Vehicle Research and Education},
year = {2021},
isbn = {9781450390453},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3483845.3483846},
doi = {10.1145/3483845.3483846},
booktitle = {2021 2nd International Conference on Control, Robotics and Intelligent System},
pages = {1–5},
numpages = {5},
location = {Qingdao, China},
series = {CCRIS'21}
}
```
This work has been published in **2021 International Conference on Control, Robotics and Intelligent System (CCRIS).** The publication can be found on [ACM Digital Library](https://dl.acm.org/doi/abs/10.1145/3483845.3483846).
