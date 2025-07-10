🗓 Daily Progress Log
Start Date: July 10, 2025  
Engineer: El Hatimi Zakaria  

---

✅ Tasks Completed

- ✅ Created initial project folder structure:
  - data/, results/, logs/
  - Placed raw .tif & .avi samples in data/raw/
- ✅ Cloned and reviewed cellpose4 + SAM segmentation notebook
- ✅ Installed required packages and validated environment (see requirements.txt)
- ✅ Started customizing cellpose_sam_spheres.ipynb
  - Loaded test .tif images
  - Initialized SAM + Cellpose models
  - Drafted segmentation pipeline and visual overlay logic

---

🔧 Technical Notes

- Verified compatibility between Cellpose 2.2.1 and SAM
- Used opencv-python to handle AVI I/O
- Configured masks per 4 classes:
  - Class 1: Circular live cells
  - Class 2: Fixed cells
  - Class 3: Post-fixation dead cells
  - Class 4: Fragments
- Output masks shape and intensity profiles logged for refinement

---

🚧 Pending Tasks 

- Add per-frame mask classification logic
- Measure brightness and area per cell
- Export metrics to metrics.csv
- Generate overlay and masked .avi videos

---

⚠ Notes / Issues

- All dependencies are documented in requirements.txt.
- Placeholder for results/metrics.csv prepared.
- Final .avi generation will use imageio and cv2 overlay functions.
