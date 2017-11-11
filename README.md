# FaceDetectionAndTracking

The is project is for detecting a face using the Viola-Jones detector and tracking it using Kalman, 
CAMShift and Particle Filters. Also implamented an Optical Flow tracker.

The logic is as follows:
 1. Detect the face in the first frame of the movie using pre-trained Viola-Jones detector
 2. Track the face throughout the movie using:
    a) CAMShift
    b) Particle Filter
    c) Face detector + Kalman Filter (always run the kf.predict(), and run kf.correct() when you get a new face detection)
 3. Additionally, implemented Face Detector + Optical Flow tracker (used the OF tracker whenever the face detector fails)
