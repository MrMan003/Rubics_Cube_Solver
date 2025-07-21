# Rubics_Cube_Solver 

Rubics_Cube_Solver is a Python-based computer vision project that scans a real Rubik’s Cube using a webcam, detects each face's colors, and solves the cube using the Kociemba algorithm. The program guides the user through each rotation step with real-time feedback.

---

## 🔧 Features

- Live video feed using OpenCV
- Face and color detection using contour analysis
- Automatic face state recognition
- Color mapping and cube state construction
- Integration with `kociemba` for optimal solving
- Step-by-step solving instructions
- Optional video recording of the solving process

---

##  Requirements

Make sure the following Python packages are installed:

```bash
pip install opencv-python numpy scipy kociemba
````

You may also need:

```bash
pip install opencv-contrib-python
```

---

##  File Structure

```
Rubics_Cube_Solver/
│
├── main.py                 # Main script to run the solver
├── rotate.py               # Contains cube rotation simulation logic
├── README.md               # This file
```

---

##  How to Use

1. **Run the program:**

   ```bash
   python main.py
   ```

2. **Follow on-screen prompts:**

   * Show each face of the cube one by one (Front, Top, Down, Right, Left, Back).
   * Make sure the cube is well-lit and centered in the camera frame.

3. **Watch the solution steps:**

   * The program will compute the optimal sequence of moves.
   * Instructions will be displayed on the video feed.

---

##  Color Mapping (Default)

| Color  | ID |
| ------ | -- |
| White  | 1  |
| Yellow | 2  |
| Red    | 3  |
| Green  | 4  |
| Blue   | 5  |
| Orange | 6  |

---

##  Notes

* Ensure uniform lighting for accurate color detection.
* You can quit anytime by pressing `ESC` or `q`.
* The `rotate.py` file must be present and correctly implemented.

---

##  Output

A video named `OUTPUT5.avi` will be saved during the process showing the scanning and solving sequence.

---

##  Credits

* Computer Vision: [OpenCV](https://opencv.org/)
* Solver: [kociemba Python Library](https://pypi.org/project/kociemba/)

---
