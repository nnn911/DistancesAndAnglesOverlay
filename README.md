# Measure Distances And Angles Overlay
Measure both distances and angles between particles and display them as an overlay in the viewport.

## Description
TBD

## Parameters 

| GUI name                     | Python name             | Description                                                                                                                                                                                                                                                                                                                                                   | Default Value     |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|
| **Particle IDs**             | `particle_ids`          | List of *particle identifiers* used as modifier input. The list is traversed in order and distances are measured between consecutive particles. If the last particle is equal to the first one, all interior angles will be measured. If *particle identifiers* are not present in the current data collection *particle indices* will be used as a fallback. | `[]`              |
| **Line width**               | `line_width`            | Width (in pixel) of all lines.                                                                                                                                                                                                                                                                                                                                | `3`               |
| **Line color**               | `line_color`            | Color of all lines.                                                                                                                                                                                                                                                                                                                                           | `(0.0, 0.0, 0.0)` |
| **Font size**                | `font_size`             | Font size for all text labels.                                                                                                                                                                                                                                                                                                                                | `0.05`            |
| **Text color**               | `text_color`            | Text color for all texts.                                                                                                                                                                                                                                                                                                                                     | `(0.0, 0.0, 0.0)` |
| **Outline width**            | `outline_width`         | Width (in pixel) of the text outline. A width of `0` corresponds to no outline.                                                                                                                                                                                                                                                                               | `0`               |
| **Show distances**           | `show_distances`        | Show distances between particles.                                                                                                                                                                                                                                                                                                                             | `True`            |
| **Number format (distance)** | `distance_label_format` | Format specifier for the particle-particle distances.                                                                                                                                                                                                                                                                                                         | `"{:.3f}"`        |
| **Show angles**              | `show_angles`           | Show angles between particles.                                                                                                                                                                                                                                                                                                                                | `False`           |
| **Arc distance**             | `arc_distance`          | Distance (in % of the particle-particle distance) in which the arc indicating the angles is displayed.                                                                                                                                                                                                                                                        | `0.2`             |
| **Number format (angles)**   | `angle_label_format`    | Format specifier for the angle measurements.                                                                                                                                                                                                                                                                                                                  | `"{:.1f} °"`      |


## Example

![Measure Distances And Angles Overlay 01](examples/Example01.png)
![Measure Distances And Angles Overlay 02](examples/Example02.png)

## Installation
- OVITO Pro [integrated Python interpreter](https://docs.ovito.org/python/introduction/installation.html#ovito-pro-integrated-interpreter):
  ```
  ovitos -m pip install --user git+https://github.com/ovito-org/DistancesAndAnglesOverlay.git
  ``` 
  The `--user` option is recommended and [installs the package in the user's site directory](https://pip.pypa.io/en/stable/user_guide/#user-installs).

- Other Python interpreters or Conda environments:
  ```
  pip install git+https://github.com/ovito-org/DistancesAndAnglesOverlay.git
  ```

## Technical information / dependencies
- Tested on OVITO version 3.9.2

## Contact
Daniel Utt utt@ovito.org