# 🃏 Augmented Reality with ArUco Markers

A Python-based augmented reality application that uses **OpenCV** and **NumPy** to 
project 3D `.obj` models onto tracked physical surfaces via **ArUco markers**.

---

## 🚀 Getting Started

### 📁 Setup Instructions

1. **Add Your Marker**
   - Copy the image of the ArUco marker you'd like to use into the `reference/` folder.
   - Show it in the openCV to detect the aruco marker 

2. **Update the Marker Reference**
   - Open `src/3Daugmented.py`
   - On **line 8**, replace `'DICT_4X4_1000'` with the name of your ArUco marker Dictionary (e.g. `'cv2.aruco.DICT_4X4_1000'`).

3. **Configure the 3D Model**
   - In the same file:
     - On **line 22**, replace `'wolf.obj'` with the filename of the 3D model you want to render.
     - On **line 142**, adjust the `object_scale` parameter to modify the model size. 
	The default is `0.0032`, but you may need to fine-tune this value.

4. **Run the Application**
   ```bash
   python src/3Daugmented.py
