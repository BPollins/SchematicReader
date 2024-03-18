# Schematic Reader Project

#### Purpose
This project aims to create a tool that construction professionals can use to automatically read mechanical schematics and tally up the number of valves. This will be useful for automated valve scheduling and for the formulation of purchase orders.
I will use the 'Reader' program to find the valves within the drawing, and then classify these with 'Classify', using a machine learning model (Ridge Classification) to identify the valve types and tally these up.

#### Progress
The program is currently able to:
- Import a single line schematic including any number of bends and branches
- Trace the line including any branches and isolate the images of the valves for identification
- Convert the image into a pandas DataFrame for classification
- Train a Ridge Classification model on the images of the valves using user-inputted labels
- Classifying the remaining valves and tallying the total for each valve type

#### Future Work
- Add the ability to trace multiple lines in the same drawing
- Improve method for finding the start position and therefore add support for uploading the bordered schematics
- Improve classification model performance

#### Data
- The program takes in sample schematics in PDF format, created using Microsoft Word
- The valve type labels used to train the model are input manually

#### System Requirements
This program is created using:
- conda 23.1.0
- jupyter 1.0.0
- jupyterlab 3.4.4
- matplotlib 3.5.2
- notebook 6.4.12
- numpy 1.23.5
- pandas 1.4.4
- pdf2image 1.16.3
- pickle5 0.0.11
- pip 22.3.1
- python 3.9.13
- scikit-learn 1.0.2
