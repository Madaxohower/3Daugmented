# 3Daugmented

A Python-based augmented reality application utilizing NumPy and OpenCV to project 3D models onto Aruco Markers dictionary.

# Setup Instruction

1. Copy the image of the surface you want to track into the reference folder.
2. In src/3Daugmented.py, on line 8, update your prepared aruco dictionary "ARUCO_DICT = cv2.aruco.getPredefinedDictionary(cv2.aruco.DICT_4X4_1000)"
3. In src/ar_main.py, on line 22, replace 'fox.obj' with the name of the 3D model you wish to display. 
4. To adjust the model’s size, modify the object_scale at line 142.
5. Open a terminal in the project directory and execute:
   '''bash python src/ar_main.py'''

# TROUBLESHOOTING
  #ERROR: "Unable to capture video"
    This typically indicates that your OpenCV installation lacks FFMPEG support. Pre-built OpenCV packages (e.g., installed via pip) often exclude FFMPEG. 
    To resolve this, you’ll need to manually build OpenCV with FFMPEG support.

# TECHNICAL DETAILS
   For a detailed explanation of the code’s logic, refer to these blog posts:
  
PART 1 (https://bitesofcode.wordpress.com/2017/09/12/augmented-reality-with-python-and-opencv-part-1/)
PART 2 (https://bitesofcode.wordpress.com/2018/09/16/augmented-reality-with-python-and-opencv-part-2/)

## Results
  In the folder '3Daugmented/Sample Image' for your reference
