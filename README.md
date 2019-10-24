# Motion Detector

Image / Video Processing using OpenCV

## Implemented using
* Python Code
* OpenCV for Video Processing
* Pandas for Data analysis
* Bokeh for Data Visualization

## Features
Processing the video from the webcam and:
* Displaying its gray version as well as normal version
* Displaying the Gaussian Blur of the video
* Displaying the object in motion as white and background as black
* Displaying Green Box around object in motion

Example : <br/>

![alt text](https://raw.githubusercontent.com/hrithikkothari1234/MotionDetector/master/Example/exampleimage.png)

## Information
Motion Detection is implemented by comparing all the frames of the video with the initial frame(i.e. frame at the beginning of the video) <br/>
Whenever an object enters the frame or leaves, datetime is generated and stored in the csv file using pandas.(To keep track) <br />
Press q to close all the windows and exit the recording. <br />
After closing all windows , a motion graph (Graph.html) is generated using the dataframe generated from the motion of the object(Bokeh is used for data Visualization here). <br /> <br />

-- This motion detector base code can be used for various purposes like Keeping a track of when a particular animal shows up OR
It can be used in raspberry pie's for motion detection.

## To run this Project go to your folder and
```
$ git clone https://github.com/hrithikkothari1234/MotionDetector.git
$ pip install cv2
$ pip install time
$ pip install pandas
$ pip install bokeh
```
After installing all dependencies
```
$ python plotting.py
```
Webcam starts and the video gets generated. <br />
Note: If you dont have a webcam , the code might throw an exception.
Note: Let the First Frame be a background that wont change at all. And then make an object enter. <br />
After quitting a Graph.html is generated which shows ur Motion Graph. <br />

* Example Graph : https://hrithikkothari1234.github.io/Webmap/Graph.html
![alt text](https://raw.githubusercontent.com/hrithikkothari1234/MotionDetector/master/Example/examplegraph.png)

![alt text](https://raw.githubusercontent.com/hrithikkothari1234/MotionDetector/master/Example/exampleimage2.png)
