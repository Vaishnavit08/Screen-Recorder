# Screen Recorder with OpenCV and PyAutoGUI

This is a simple and efficient screen recording tool implemented in Python using OpenCV and PyAutoGUI. The program captures your screen in real-time and saves the recording in the specified video file format.

## Features
- Records the entire screen with the resolution of your system.
- Customizable output file name and path.
- Adjustable frame rate for smooth recording.
- Displays a live preview of the screen being recorded.
- Saves the recording in `.avi` format using the XVID codec.

## Prerequisites
Make sure you have the following installed on your system:

- Python 3.6 or later
- Required Python libraries:
  - OpenCV (`cv2`)
  - PyAutoGUI (`pyautogui`)
  - NumPy (`numpy`)

You can install the required libraries using pip:
```bash
pip install opencv-python pyautogui numpy
```

## How to Use

1. Clone this repository or copy the `screenrecorder.py` file.
2. Run the script using Python:
   ```bash
   python screenrecorder.py
   ```
3. Enter the file name and path where you want to save the recording. For example:
   ```
   Enter your file name and path: C:\Users\Vaishnavi\Desktop\recording.avi
   ```
4. The recording starts immediately, and a live preview window named **Live_Recording** will appear.
5. To stop the recording, press the `v` key.
6. The recorded video will be saved to the specified location.

## Code Overview

### Imports
- `cv2`: For video processing and handling.
- `pyautogui`: To capture the screen.
- `numpy`: For handling image arrays.

### Main Functionalities
- **Resolution Setup**: The screen resolution is dynamically fetched using `pyautogui.size()`.
- **Custom File Name**: The user inputs the file name and path.
- **Live Preview**: The program displays a resizable window showing the live screen being recorded.
- **Recording Loop**: The screen is captured using `pyautogui.screenshot()`, converted to an OpenCV-compatible format, and written frame by frame to the output file.
- **Exit Mechanism**: The recording stops when the `v` key is pressed, releasing resources and closing the window.

## Example Output
Below is an example of running the program:

```plaintext
Enter your file name and path: C:\Users\Vaishnavi\Desktop\recording.avi
```

This will save the screen recording as `recording.avi` on your desktop.

## Note
- Ensure the file path and name are valid and writable.
- Adjust the frame rate (`fps`) for optimal performance based on your system's capabilities.

## Future Improvements
- Add support for pausing and resuming recording.
- Include options for recording specific regions of the screen.
- Add an audio recording feature.

## Contributing
If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Contributions are welcome!

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

### Author
[Vaishnavi Pravin Talekar](https://github.com/Vaishnavit08)

Feel free to check out my other projects on [GitHub](https://github.com/Vaishnavit08)!
