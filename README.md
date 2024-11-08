# Football Analysis

This project aims to detect and track players, referees, and footballs in video footage using the YOLO object detection model. It includes team assignment based on t-shirt colors using Kmeans clustering, movement analysis with optical flow, and perspective transformation to measure player movements accurately.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)
- [Requirements](#requirements)
- [Screenshot](#screenshot)
- [Trained Models](#trained-models)
- [Sample Video](#sample-video)

## Introduction

The goal of this project is to analyze football matches by detecting and tracking players, referees, and footballs. It uses YOLO for object detection, Kmeans for team assignment, optical flow for camera movement analysis, and perspective transformation for accurate measurement of player movements.

## Features

- **YOLO**: Detect players, referees, and footballs.
- **Kmeans**: Assign players to teams based on t-shirt colors.
- **Optical Flow**: Measure camera movement between frames.
- **Perspective Transformation**: Measure player movements in meters.
- **Movement Analysis**: Calculate player speed and distance covered.

## Usage

Run the scripts to perform various analyses:

1. **Detection and Tracking**:
    ```bash
    python scripts/detect_and_track.py --input videos/sample_input.mp4 --output results/output.mp4
    ```
2. **Team Assignment**:
    ```bash
    python scripts/team_assignment.py --input videos/sample_input.mp4 --output results/team_output.mp4
    ```
3. **Movement Analysis**:
    ```bash
    python scripts/movement_analysis.py --input videos/sample_input.mp4 --output results/movement_output.mp4
    ```

## Contributing

We welcome contributions to enhance this project! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Football Players Detection Dataset](https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc/dataset/1) from Roboflow.
- [DFL Bundesliga Data Shootout](https://www.kaggle.com/competitions/dfl-bundesliga-data-shootout/data?select=clips) from Kaggle for the data.
  
## Requirements

To run this project, you need to have the following installed:

- Python 3.x
- Ultralytics
- Supervision
- OpenCV
- NumPy
- Matplotlib
- Pandas

## Screenshot
 <img width="1705" alt="Screenshot 2024-06-25 at 5 18 43 PM" src="https://github.com/jjc98375/football-analysis/assets/62311247/aced5ef3-d5f1-4c5c-95e9-9ef4aa0c84f2">


## Trained Models

- [Trained YOLO v5](https://github.com/jjc98375/football-analysis/blob/main/models/best.pt)

## Sample Video


- [sample video](https://github.com/jjc98375/football-analysis/assets/62311247/5dc62030-2432-4881-9244-3091b2117b79)

