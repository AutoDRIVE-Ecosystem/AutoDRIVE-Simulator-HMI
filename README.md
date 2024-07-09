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
