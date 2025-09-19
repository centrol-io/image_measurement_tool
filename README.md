# Image Measurement Tool

A powerful, browser-based application for performing precise measurements on images. This tool allows users to set a reference scale and then draw lines to measure lengths and determine coordinates relative to a user-defined origin. It's built as a single, self-contained HTML file, making it incredibly easy to use and deploy.

* Live Demo Link: *

## Features

This tool is packed with features to ensure a precise and user-friendly measurement experience:

- Multiple Image Import Options:
  - Upload: Select a local image file.
  - Drag & Drop: Drag an image directly into the application.
  - Paste Image: Copy an image (e.g., a screenshot) and paste it with Ctrl+V.
  - Paste URL: Paste a direct URL to an image.

- Calibration & Scaling:
  - Draw a reference line on an object of known length to set a precise scale for all subsequent measurements.
  - Select from a dropdown of common units (mm, cm, in) or use pixels.

- Measurement & Analysis:
  - Draw multiple measurement lines on the image.
  - Instantly view the length and midpoint of each line.
  - Set a "Home Position" (origin point) to calculate the coordinates of each line's start, mid, and end points relative to it.

- Advanced Canvas Controls:
  - Zoom: Use the mouse wheel to zoom in and out for pixel-perfect accuracy.
  - Pan: Hold the spacebar and drag the mouse to move around the image.

- Interactive Editing:
  - Enter the dedicated "Edit Lines" mode to modify your work.
  - Move Lines: Drag any line from its body to a new position.
  - Resize Lines: Drag the circular handles at the start or end of a line to adjust its length and angle.

- Data Export:
  - Save all your measurement data (scale, units, home position, and all line coordinates) to a local JSON file for offline access or future use.

## How to Use

1. Load an Image: Start by getting an image onto the canvas using one of the four import methods.

2. Set the Scale (Crucial First Step):
  - The app will start in "Set Reference Scale" mode.
  - Find an object of a known length in your image.
  - Click and drag to draw a line along that object.
  - When you release the mouse, a dialog will appear. Enter the known length and select the correct unit from the dropdown. Click "Set Scale".

3. Draw Measurement Lines:
  - The app will automatically switch to "Draw Measurement Line" mode.
  - Click and drag anywhere on the image to draw lines. The info panel on the left will update with the calculated length.

4. Edit Lines (Optional):
  - Click the "Edit Lines" button.
  - Click on a line to select it. Blue handles will appear.
  - Drag the end handles to resize the line or drag the middle of the line to move it. The info panel will update in real-time.

5. Set a Home Position (Optional):
  - Click the "Set Home Position" button.
  - Click anywhere on the image to set your (0,0) origin.
  - Alternatively, after setting a scale, you can type the coordinates directly into the "Home X" and "Home Y" input fields in the selected unit.
  - The info panel will now display the coordinates for the start, mid, and end points of your lines relative to this home position.

6. Save Your Work:
  - Click the "Save Results" button at any time to download a .json file of your current session.

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.