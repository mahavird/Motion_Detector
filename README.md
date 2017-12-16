# motion-detection-with-opencv
Thanks to **Adrian Rosebrock**, he gives us a very awesome project that using Respberry Pi, Python and OpenCv to detect motion. Details you can read this website:[Home Surveillance](http://www.pyimagesearch.com/2015/06/01/home-surveillance-and-motion-detection-with-the-raspberry-pi-python-and-opencv/).

I have fine tuned ported this project for detecing a motion for an a video stream based on IP Camera.

### hardware
- Linux based System
- HK Vision IP Camera
    Output resoultion of video stream from camera  --  1920 x 1080
    Codec -- H264

### software
- Python
- OpenCV
- imutils

### steps
#### 1. Download source code
```bash
$ git clone https://github.com/mahavird/Motion_Detector
```
### 2. Provide the input source:
Thanks to openCv you can use the same code for live streaming videos, comment/uncomment the desired input source for use case.
In the file "motion-detector.py", you can find the lines similar to:
        video_capture = cv2.VideoCapture("test_stable.mp4")
Do make the necessary changes.

### 3. Test
```bash
$ python motion-detector.py -c conf.json
```

