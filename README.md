# AutoDRIVE Simulator HMI
Human Machine Interfaces to AutoDRIVE Simulator

![Framework](Media/Framework.jpg)

## Human Machine Interfaces

**Observation Interfaces:**
- Single Monitor
- Triple Monitor
- XR Headset

**Interaction Interfaces:**
- Keyboard
- Mouse/Trackpad
- Gamepad
- Driving Rig

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

## User Study

We administered the immersive presence of 16 users within the virtual environment of the proposed framework using the Bob G. Witmer Presence Questionnaire (PQ) [[25]](https://doi.org/10.1162/105474698565686), [[26]](https://doi.org/10.1162/105474605323384654). The questionnaire is made available as [Presence Questionnaire.xlsx](User%20Study/Presence%20Questionnaire.xlsx) and the user demographics are recorded in [Demographics.xlsx](User%20Study/Demographics.xlsx). Individual user responses for various observation and interaction interfaces are stored as `CSV` files within the [User Study](User%20Study) directory and are post-processed using the [data_analysis.mlx](User%20Study/data_analysis.mlx) script. Following are the post-processed user experience analyses for observation and interaction interfaces:

**Observation Interfaces:**
![User experience analyses for observation interfaces](User%20Study/data_analysis_observation.png)

**Interaction Interfaces:**
![User experience analyses for observation interfaces](User%20Study/data_analysis_interaction.png)

## Case Study

In order to evaluate the serviceability of the proposed framework, an edge-case urban driving scenario was devised. The scenario was laid out to jump-scare the ego vehicle and analyze its reactive response to the event. Particularly, the ego vehicle was supposed to keep driving straight unless it was unsafe/unethical to do so (e.g. dead end, traffic sign, traffic light, imminent collision, etc.). Down the road, a semiautonomous virtual vehicle was set up to cut across the ego vehicle as it approached the first 4-way intersection, requiring the ego vehicle to execute a panic-breaking maneuver while ensuring safety in case of any failures. The following plot depicts the ego vehicle behavior in autonomous (AV), connected autonomous (CAV), human-operated with static HMD (HV-S), and human-operated with dynamic HMD (HV-D) modes of operation:

![Ego vehicle behavior for panic-breaking case study](/Case%20Study/data_analysis.png)
