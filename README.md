

Reference:

https://github.com/ultralytics/xview-yolov3/blob/main


Git check in:

===

A.Set Up Environment:

1. Install Python
Ensure that Python is installed on your system. You can verify this by opening a terminal/command prompt and typing:

python --version
If Python is not installed, you can download it from the official Python website.

2. Install the Python Extension in VSCode
If you haven't installed the Python extension in VSCode yet, follow these steps:

Open VSCode.
Go to the Extensions panel (click on the Extensions icon in the left sidebar or press Ctrl+Shift+X).
Search for Python and install the one by Microsoft.
After installation, reload VSCode if necessary.
3. Create a Virtual Environment
Follow these steps to create and activate a virtual environment in your project directory:

1. Open the Integrated Terminal
In VSCode, open the integrated terminal by pressing Ctrl+ or navigating to Terminal > New Terminal from the menu.
2. Create a New Project Folder (If Necessary)
You can create a new folder for your project using the terminal:

mkdir my_project
cd my_project
3. Create a Virtual Environment
To create a virtual environment using the venv module:

Run the following command in the terminal (make sure you're in the project folder):

python -m venv venv
This will create a folder named venv in your project directory containing the virtual environment.
4. Activate the Virtual Environment
Once the virtual environment is created, you need to activate it. The activation command differs depending on your operating system.

Windows:

.\venv\Scripts\Activate
macOS/Linux:
bash
Copy
source venv/bin/activate
After activation, you should see the virtual environment name (venv) in your terminal prompt, indicating that the virtual environment is active.

B. Download YOLO Model Weights and Configuration
For object detection, we'll use the YOLOv3 pre-trained model, which is available on the official YOLO website or GitHub. You'll need:

YOLOv3 weights file: yolov3.weights
YOLOv3 configuration file: yolov3.cfg
coco.names: The file that contains the names of the objects the model is trained to recognize (e.g., person, car, dog, etc.).
You can download the yolov3.weights, yolov3.cfg, and coco.names from the following links:

YOLOv3 Weights
YOLOv3 Config
Coco Names


C. Implement the Object Detection Code

Here’s a Python script that uses OpenCV and YOLOv3 to detect objects in a video file.

object_detection_video.py

sample video file : 853889-hd_1920_1080_25fps.mp4


D. Check in the code Git


echo "# deeplens_object_detection_poc" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/ramkotni/deeplens_object_detection_poc.git
git push -u origin main






