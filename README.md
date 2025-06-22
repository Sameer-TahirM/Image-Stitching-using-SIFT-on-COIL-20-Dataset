# Computer Vision Projects: SIFT Panorama and Hough Transform Chess Game

## 📖 Description

This repository contains two distinct computer vision projects demonstrating fundamental and advanced techniques in image processing.

1.  **SIFT Image Stitching**: This project implements the Scale-Invariant Feature Transform (SIFT) algorithm from scratch to create panoramic images. Using the COIL-20 dataset, it intelligently selects and stitches 15 images for each of the 20 objects to form a coherent panorama.

2.  **Chess Game Simulation**: This project uses the Hough Line Transform to detect the grid of a chessboard. It then calculates line intersections to identify the 64 squares, places chess pieces onto the board, and applies projective transformations to create a dynamic, 3D-like view of the game.

## ✨ Features

### Project 1: SIFT Image Stitching
-   **Feature Detection**: Implements the SIFT algorithm to detect and match keypoints between multiple images.
-   **Panorama Generation**: Stitches 15 images for each of the 20 objects in the COIL-20 dataset.
-   **Image Selection**: Intelligently selects the best-suited images from 72 available angles to ensure a smooth and logical panoramic output.

### Project 2: Chess Game Simulation
-   **Line Detection**: Uses the Hough Line Transform to accurately detect the grid lines of a chessboard.
-   **Board Analysis**: Calculates line intersection points to programmatically identify and count the 64 squares on the board.
-   **Object Placement**: Simulates placing chess pieces by replacing the pixels within the detected squares with the piece's image.
-   **3D Transformation**: Applies projective transformations to the chessboard to create a dynamic 3D-like perspective.



## 🚀 Getting Started

Follow these instructions to set up the project on your local machine.

### Prerequisites
-   Python 3.8+
-   `pip` package manager

### Installation
1.  Clone the repository:
    ```sh
    git clone https://github.com/your_username/your_repo_name.git
    cd your_repo_name
    ```
2.  Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```
3.  Download the **COIL-20 dataset** from [Kaggle](https://www.kaggle.com/datasets/cyx6666/coil20) and place the contents in the `data/coil-20/` directory.

## 💻 Usage
The project is split into two main components. Run the corresponding script or notebook to execute each part.

-   **Image Stitching**:
    ```sh
    python image_stitching.py
    ```
-   **Chess Game Simulation**:
    ```sh
    python chess_game.py
    ```
The output panoramas will be saved in the `output/panoramas/` directory.

## 🛠️ Technology Stack
-   **Python**
-   **OpenCV (`cv2`)**: For SIFT, Hough Transforms, and image transformations.
-   **NumPy**: For numerical operations and array manipulation.
-   **Matplotlib**: For displaying images and results.

## 💾 Dataset
1.  **COIL-20 Dataset**: Used for the image stitching project. This dataset contains 72 grayscale images for each of 20 objects, with each image captured at a 5-degree rotational interval.
2.  **Chess Assets**: The chessboard simulation uses a standard chessboard image and individual PNG files for each chess piece, located in the `images/` directory.
