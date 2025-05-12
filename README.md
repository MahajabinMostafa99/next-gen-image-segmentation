# Next-Generation Image Segmentation and Object Detection

This is my final project for the **Digital Image Processing** course. The project applies advanced deep learning techniques to perform **brain tumor segmentation** and **object detection** on MRI slices. A U-Net model is used for segmentation, while a custom detection model predicts bounding boxes. A **Gradio demo** is also included for interactive testing.

---

## Highlights

- **Dataset:** BRATS 2020 (Brain Tumor Segmentation Challenge)  
- **Models Used:**
  - `U-Net` for pixel-wise tumor segmentation
  - Custom CNN model for object detection
- **Evaluation Metrics:** Dice Score, IoU
- **Tools:** TensorFlow, Keras, OpenCV, Gradio
- **Demo Interface:** Gradio UI for real-time testing

---
###  Folder Structure

<pre>
next-gen-image-segmentation/
├── NextGenImageSegAndObjDet.ipynb
├── Gradio_Demo/
│   ├── demo_seg_detect.py
│   ├── volume_9_slice_66.h5
│   ├── volume_211_slice_51.h5
│   ├── volume_340_slice_78.h5
│   ├── unet_best.h5 (add it after generating)
│   └── best_detector.iou.h5  (add it after generating)
├── README.md
</pre>

---
## How to Run

### Step 1: Run the Notebook

Open and execute `NextGenImageSegAndObjDet.ipynb` (in Colab or locally).  
This notebook will:
- Train both segmentation and detection models
- Automatically generate:
  - `unet_best.h5`
  - `best_detector.iou.h5`
- Save them to the `Gradio_Demo/` folder

---

### Step 2: Run the Gradio Demo

After running the notebook:

```bash
cd Gradio_Demo
python demo_seg_detect.py
