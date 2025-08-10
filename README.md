
# CCTV Footage Person Detection

This project detects and tracks persons in CCTV footage using YOLOv8 for object detection and ByteTrack for multi-object tracking.
It assigns unique IDs to each person using Torch ReID, logs their entry and exit timestamps into a CSV file, and produces an annotated output video with bounding boxes and IDs.


## Project Structure
The input_video and output_video may not be visible directly inside Github, but they can be downloaded and then can be seen. I have removed the outputs from the code.ipynb file, in order to check the outputs, the link https://colab.research.google.com/drive/1AuNaZHjei1uKkbyO2xwgdkGDVZ1tMJ_O?usp=sharing  can be checked.
```
├── code.ipynb
├── byte_tracker.py
├── input_video.mp4
├── output_video.mp4
├── log.csv
└── README.md
```
## Input and Output
A video (generally taken from CCTV footage) is given as input to my model. As output, it then gives a .csv log file showing time stamp of entry and exit of each person in hh:mm:ss and a video showing bounding boxes around each person detected in input video is formed.
## Requirements and Installation
In this project following modules were installed. These installations are mostly done automatically in the code but only the byte_tracker.py file of yolox folder inside the ByteTrack folder is edited. The edited file is also provided.

    1) Python 3.8+

    2) Google Colab (GPU runtime recommended)

    3) Ultralytics YOLOv8

    4) ByteTrack

    5) Supervision

    6) TorchReID
