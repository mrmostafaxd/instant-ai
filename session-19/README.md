# Session 19 Tasks

## Task 1

Mention 5 computer vision package.

### Solution

-   [YOLOv8](https://medium.com/cord-tech/yolov8-for-object-detection-explained-practical-example-23920f77f66a)
-   [SimpleCV](http://simplecv.org/)
-   [Deepface](https://github.com/serengil/deepface)
-   [BoofCV](https://boofcv.org/index.php?title=Main_Page)
-   [Torchvision](https://pytorch.org/vision/stable/index.html)

[(return to top)](#session-19-tasks)

## Task 2

Read real-time video with audio simultaneously.

### Solution

`av_record` is a Python script that simultaneously records audio and video using threading. The audio and video are recorded separately for better performance. The script is inspired by JRodrigoF's [script](https://github.com/JRodrigoF/AVrecordeR)

The script was tested on Windows 11 operating system.

<br>
To run the `av_record` script, open the terminal or command prompt and use the following command:

```shell
python .\testrunning.py {video_name} --sleep_time {duration}
```

Replace `{video_name}` with the desired name of the final video file (without the file extension), and `{duration}` with the recording duration in seconds. The script will record both audio and video for the specified duration and then merge them into a single final video file.

Please make sure you have the necessary dependencies (OpenCV, pyaudio, wave, ffmpeg) installed before running the script.

[(return to top)](#session-19-tasks)

## Task 3

Real-time face detection using [MediaPipe](https://developers.google.com/mediapipe)

### Solution

`face_detection` is a script that utilizes OpenCV and MediaPipe to overlay a rectangle over the detected faces in real-time.

The script was tested on Windows 11 operating system.

<br>
To run the script, open the terminal or command prompt and use the following command:

```shell
python .\face_detection.py
```

Please make sure you have the necessary dependencies (OpenCV, MediaPipe) installed before running the script.

[(return to top)](#session-19-tasks)
