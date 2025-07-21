## Author
This project was built by Nikesh Kumar.
contact: nikeshkumar310305@gmail.com

# Colorization Project

This project implements image colorization using deep learning models. It uses pre-trained models (`ECCV16` and `SIGGRAPH17`) to colorize grayscale images.

## Features
- Supports GPU acceleration for faster processing.
- Outputs colorized images using two different models: `ECCV16` and `SIGGRAPH17`.
- Saves the results as `.png` files.

## Dependencies
The project requires the following libraries:

torch
scikit-image
numpy
matplotlib
argparse
Pillow

## Usage
Run the script demo_release.py to colorize an image.

## Command-line Arguments
-i or --img_path: Path to the input image (default: a sample image path).
--use_gpu: Use GPU for processing (optional).
-o or --save_prefix: Prefix for saving the output files (default: saved).

This will generate two output files:

output_eccv16.png
output_siggraph17.png

GitHub Copilot
Here is a sample README.md file for your project:

Dependencies
The project requires the following libraries:

torch
scikit-image
numpy
matplotlib
argparse
Pillow
Usage
Run the script demo_release.py to colorize an image.

Command-line Arguments
-i or --img_path: Path to the input image (default: a sample image path).
--use_gpu: Use GPU for processing (optional).
-o or --save_prefix: Prefix for saving the output files (default: saved).

## Key Files
demo_release.py: Main script to run the colorization.
colorizers/: Contains the models and utility functions.
eccv16.py: ECCV16 model implementation.
siggraph17.py: SIGGRAPH17 model implementation.
util.py: Utility functions for image preprocessing and postprocessing.
requirements.txt: List of required Python packages.

## Output
The script generates the following:

Original Image: The input image.
Grayscale Image: The input image converted to grayscale.
Colorized Image (ECCV16): Output from the ECCV16 model.
Colorized Image (SIGGRAPH17): Output from the SIGGRAPH17 model.