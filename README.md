# robot_path
Robot Path Detection with Obstacle Avoidance" is a Python-based simulation that models how a simple robot would navigate a 2D space (represented by an image) while avoiding obstacles.

## 🧠 Project Description

- The input image represents a map where **white regions are obstacles** and the **dark background is free space**.
- The robot starts from the **left-center** of the image.
- It moves in small steps toward the right.
- If it detects an obstacle in front, it tries to move **down** or **up** to avoid it.
- The robot’s path is plotted as a series of **green dots** on the image.

## 📁 Folder Contents

robot-path-detector/
├── robot_path.py # Main Python script
├── robot_map.jpg # Input image (map with obstacles)
├── requirements.txt # Dependencies
└── README.md # This file

## 📷 Sample Input

- The image should be a **top-down view** map.
- White or light objects represent **obstacles**.
- Background should be dark.

## 🔧 Requirements

Install dependencies:

```bash
pip install -r requirements.txt
requirements.txt content:
Copy code
opencv-python
matplotlib
numpy

▶️ How to Run
bash
Copy code
python robot_path.py
Make sure robot_map.jpg is in the same folder.

The output will be shown as a plot with the robot’s walking path in green.

📌 Notes
The robot walks from left to right across the image.

If the robot gets completely surrounded, it will stop and print a warning.

You can replace the input image with your own map by renaming it to robot_map.jpg.

🚀 Future Improvements
Add smarter path planning (A*, Dijkstra)

Visualize movement step-by-step using OpenCV

Export the path as a CSV or overlay grid navigation

🧑‍💻 Author
Made with ❤️ using Python and OpenCV
