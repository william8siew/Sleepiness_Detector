# Sleepiness_Detector
Program that takes real-time video of a person's face while they are working on a computer to determine if they are sleepy.

NEXT-UPDATE PLANS: Work on other indicators of sleepiness other than elongated eye closure. Eye rate can be calculated by keeping a heap of difference in blinking times. 

References:
https://www.researchgate.net/publication/227047615_Drowsy_Driver_Detection_Through_Facial_Movement_Analysis
"Previous approaches to drowsiness detection primarily make pre-assumptions about the relevant behavior, focusing on blink rate, eye closure, and yawning."

https://www.pyimagesearch.com/2017/04/24/eye-blink-detection-opencv-python-dlib/
Reference for non-machine learning approach of using dlibs prebuilt facial detection feature. 

http://www.diva-portal.org/smash/get/diva2:673983/FULLTEXT01.pdf
"According to Andreassi (2000), a relaxed person blinks about 15-20 times per
minute, although only 2-4 are needed from a physiological viewpoint. When performing
cognitive tasks the blink frequency drops to as little as 3 blinks per minute, whereas an
increase in blink frequency indicates reduced vigilance (Hargutt & Krüger, 2000)."
 
https://www.researchgate.net/publication/259390217_DEVELOPMENT_OF_AN_EYE-BLINK_DETECTION_SYSTEM_TO_MONITOR_DROWSINESS_OF_AUTOMOBILE_DRIVERS

## Setup the Environment

Use Python 3.6.X

## Additional Information
-Glasses may ocassionaly disrupt blink detection. The imported dlib library may mistakenly plot the points on the glasses, especially if they reflect color such as blue-light blocking glasses.
-The figures provided show the eye-aspect ratios of me performing 3 blinks followed by a slowly closing my eyes and holding it for a while(meant to represent sleepiness).
-I tested the program on three distances: 6,12, and 18 inches meant to represent leaning in at the screen, working at a normal distance, and laying against a chair respectively.
-Based on the figures, I chose 0.18 as the eye-aspect ratio for eyes being closed and 10 consecutive frames as too long for one's eyes to be closed.






