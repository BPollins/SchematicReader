### Purpose
This project aims to create a tool that construction professionals can use to automatically read mechanical schematics and tally up the number of valves. This will be useful for automated valve scheduling and for the formulation of purchase orders.
I will use the 'Reader' program to find the valves within the drawing, and then classify these with 'Classify' - using a machine learning model (Support Vector Classification) to identify the valve types and tally these up.

### Progress
The program is currently able to:
- Import a single line schematic including any number of bends
- Trace the line, isolating the images of the valves in the line for identification
- Train an SVC model on the images of the valves using user-inputted labels
- Classifying the remaining valves and tallying the total for each valve type

### Future Work
- Add the ability to identify and navigate branches in the schematic (not just single-lines)
- Add the ability to trace multiple lines in the same drawing
- Improve method for finding the start position and therefore add support for uploading the bordered schematics
- Improve classification model performance
