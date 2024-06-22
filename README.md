# Image Compression using K-Means Clustering

This project demonstrates an image compression technique using the K-Means clustering algorithm. The original image is compressed by reducing the number of unique colors, which can significantly decrease the image file size while maintaining visual quality.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Image compression is a process of reducing the file size of an image while preserving its quality. This project utilizes the K-Means clustering algorithm to achieve compression by clustering similar colors and reducing the number of unique colors in the image.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/CGbhakt420/Image-Compression.git
    cd Image-Compression
    ```

2. Install the required dependencies:
    ```bash
    pip install numpy matplotlib 
    ```

## Usage

1. Place the image you want to compress in the project directory and update the `image_path` variable in the script.

2. Run the script:
    ```bash
    python compress_image.py
    ```

## Code Explanation

### Functions

- `find_closest_centroids(X, centroids)`: Finds the closest centroids for each data point in X.
- `compute_centroids(X, idx, K)`: Computes new centroids based on the current cluster assignments.
- `kMeans_init_centroids(X, K)`: Initializes centroids by randomly selecting K data points from X.
- `run_kMeans(X, initial_centroids, max_iters=10, plot_progress=False)`: Runs the K-Means algorithm for a given number of iterations.

### Main Code

1. Load and normalize the image.
2. Reshape the image data for clustering.
3. Initialize and run the K-Means algorithm.
4. Reconstruct the compressed image from the cluster centroids.
5. Display and compare the original and compressed images.

## Results

The compressed image uses fewer colors but retains a high level of visual fidelity compared to the original image. Here is an example of the results:

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License


