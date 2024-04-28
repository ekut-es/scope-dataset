# Scope Dataset Toolkit (available soon)

![Scope-Logo](images/scope_high_res.png)

Here you can download the official Toolkit for the [SCOPE dataset](https://ekut-es.github.io/scope/).
The Toolkit provides functionality for an efficient parallel download, visualization and evaluation of Collective Perception Algorithms.

![Toolkit](images/Toolkit.png)

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the Toolkit.

```bash
pip install scope-toolkit
```

## Usage
Once installed, you can start using the Toolkit to enhance your workflow with the SCOPE dataset. 

### Download

The Toolkit allows efficient parallel downloading and extraction into the correct structure of the SCOPE dataset.

Simply run 
```
cd ~/dataset-toolkit
python dataset-toolkit/TODO_ADD_PATH_TO/download_dataset.py
```
and follow the on-screen instructions.


### Visualization

![Visualization_Cam+LiDAR](images/243_in_2021_08_23_21_47_19_CamLidar.gif)
![Visualization_45Top](images/243_in_2021_08_23_21_47_19_45Top.gif)

The visualization module allows for an easy exploration of the dataset.

To visualize a scenario run
```
cd ~/dataset-toolkit
python dataset-toolkit/TODO_ADD_PATH_TO/visualize_sequence.py
```
and follow the on-screen instructions.
This will create a GIF of the selected scenario while following the selected car in the given scenario.

Currently there are a few different perspectives implemented. Those are

```mermaid
    graph TD
        A{Viewpoint} -->|third-person/roof Camera+LiDAR| B(roof-option)
        A --> |bird's eye view 45° only LiDAR| C[GIF]
        B -->|front view| D(camera alignment)
        B -->|front to back| E(camera alignment)
        D --> |next to| F[GIF]
        D --> |above| G[GIF]
        E --> |next to| H[GIF]
        E --> |above| I[GIF]
```

### Evaluation (TODO)
Evaluation module for easy and fair comparison of different methods using state-of-the-art metrics
TODO

## Roadmap

## Contributing

## Authors and acknowledgment

## License

## Project status

## Citation