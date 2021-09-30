# handGestureVolumeControl
Developed a hand gesture volume control model using opencv.
Title: Volume Controller using Hand Detection

Aim: To study Application of Digital Signal Processing (Mini project)

INTRODUCTION:

Gesture Detection can have multiple real-world applications. One such useful application can be Hand Detection which can be used in many specific software. A more specific example could be Controlling the volume of the system according to the movement of fingers. This topic can have multiple applications like controlling volume through fingers rather than manually while watching a movie or any program, controlling the volume of music system conveniently through fingers while driving. This system helps make the process of controlling volume much simpler. This system can be used as a part of some software or it can even be integrated with an audio playing hardware.
BACKGROUND:
Volume control using hand detection has a variety of applications. If implemented with musicsystems can change the way of controlling sound without actually wanting to physically 
interact with the system. So, we are developing such kind of project which adjusts the volume of the system based on the adjustments of the thumb and index finger. 
PROBLEM STATEMENT:
In this project, the problem statement is “To develop a volume controller project which adjusts the volume of the system based on the adjustments made by the thumb and index finger"

LITERATURE SURVEY:
A]	Existing System Survey:
ANN for Gesture Recognition using Accelerometer Data : The authors introduced an Artificial Neural network application used for the classification and gesture recognition. The gesture recognition is done through the Wii remote, this remote will rotate in X,Y,Z directions. To reduce the computational cost and memory consumption the gesture recognition is processed in two levels. In first level User Authentication is done for gesture recognition. Accelerometer- Based gesture recognition method is used .In second level without any kind of signal processing for gesture recognition Fuzzy automata algorithm has been proposed. After recognizing the data of the gestures, the data was normalized and filtered by k-means and Fast Fourier transform algorithm. Using this Dynamic Bayesian Network The recognition accuracy has increased up to 95%.
Combining multiple depth-based descriptors for hand gesture recognition: Based on the depth information of the image taken by the depth cameras the authors have introduced a scheme known as novel hand gesture recognition scheme. To properly recognize complex gestures by using 3-D information they used a set of 3-Dimensional features. The proposed hand gesture recognition system consist of three main steps .The first step based on colour and depth information the hand samples are segmented from the background. Wrist samples, palm and the fingers are subparts of the segmented hand samples. The proposed hand gesture recognition consists of four types of features. The second step is to extract these features for the segmentation. The first two set of features are based on the distance from elevation of finger tips to palm center. The third feature set concentrate on computed curvature features of hand contour. The fourth set is on constructed geometry of the palm region. The SVM classifier is used with constructed feature vectors to identify the hand gesture which is performed in front of the camera .The accuracy of 95% is achieved with the combination of feature set and the SVM classifier.
B]	Existing System Limitations:
Hand Gesture is an active area of research in the vision community, mainly for the purposes of sign language recognition and human-computer interaction. One of the original tracking systems to focus on articulated hand motion was present. In their system, a 27 degree-of- freedom hand could be tracked at 10Hz by extracting point and line features from grayscale images. However, it has difficulty tracking in the presence of occlusions and complicated backgrounds, and it requires a manual initialization step before tracking can begin.
C]	Project Contribution:
We have created a project which helps make the process of adjusting the volume of the system easier through adjustment of the length between index finger and thumb

IMPLEMENTATION:
We have implemented the project using python programming language. The project consists of a file named HandTrackingModule which tracks the position of the hand from the display
 
shown in the camera and detects the position of the fingers. The libraries used in HandTrackingModule are cv2 which is used for image recognition and mediapipe which is used for creating customizable ML solutions for live and streaming media.
The position of the located fingers in then using by the file VolumeHandController which selects the position of only thumb and index finger. The function of changing the volume of the system done by this file according to the selected positions of index finger and thumb. It uses the library pycaw which is a Python Core Audio Windows Library, it helps to set the range of volume based on the range of the distance between the two fingers. comtypes which is used to implement both custom and dispatch based COM interfaces.

OUTPUT:
![image](https://user-images.githubusercontent.com/58439134/135482161-48e2846f-019e-45f3-8299-2a95c55115cc.png)

![image](https://user-images.githubusercontent.com/58439134/135482201-aaf6ff23-6f57-4187-aa08-9134a38449dd.png)


CONCLUSION:
Thus we have created a volume controller which controls volume of system based on the adjustment of length between index finger and thumb which it detects through the view of the camera.


REFERENCES:
1.	Akira Utsumi, TsutoniuMiyasato, Fumio KishinoandRyoheiNakatsu, “Real-time Hand Gesture RecognitionSystem,” Proc. of ACCV ’95, vol. 11, pp. 249-253, Singapore,1995
2.	Attila Licsár, TamásSzirányi University of Veszprém, “Dynamic Training of Hand Gesture Recognition System” Department of Image Processing andNeurocomputing, H8200 Veszpré,23-26 Aug. 2004
3.	L. Bretzner and T. Lindeberg, “Relative orientation from extended sequences of sparse point and line correspondences using the affine trifocal tensor,” in Proc. 5th Eur. Conf. Computer Vision, Berlin, Germany, June 1998, vol. 1406, Lecture Notes in Computer Science, pp.141–157, Springer Verlag
4.	Intel Corp, “OpenCV Wiki,” OpenCV Library [Online], Available: http://opencv.willowgarage.com/wiki /
5.	Z. Zhang, Y. Wu, Y. Shan, S. Shafer. Visual panel: Virtual mouse keyboard and 3d controller with an ordinary piece of paper. In Proceedings of Perceptual User Interfaces, 2001
6.	W. T. Freeman and M. Roth, Orientation histograms for hand gesture recognition. International workshop on automatic face and gesture recognition. 1995, 12: 296- 301.
7.	G. R. S. Murthy, R. S. Jadon. (2009). “A Review of Vision Based Hand Gestures Recognition,” International Journal of Information Technology and Knowledge Management, vol. 2(2), pp. 405410.
8.	Mokhtar M. Hasan, Pramoud K. Misra, (2011). “Brightness Factor Matching For Gesture Recognition System Using Scaled Normalization”, International Journal of Computer Science & Information Technology (IJCSIT), Vol. 3(2).
