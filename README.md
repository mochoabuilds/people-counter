# People-Counter

* Outline area around humans entering/exiting a building with a rectangle and update total number inside building accordingly.

## 01 Installing Required Packages and Libraries

    Python
    OpenCV - https://opencv.org/
    dlib - http://dlib.net/a

## 02 "The Recipe"

* This code planning and development was based on a pre-trained MobileNet SSD object detector, dlib's correlations tracker and my own centroid tracking recipe (accepting bounding box coordinates, computing centroids, computing Euclidean distance between new bounding boxes and existing, updating coordinates of exisiting object, registering new objects and deregistering old/lost object out of the frame).

## 03 Footfall/People Counter (See Attached Code)

    Videos/
        .avi
        .mp4
        .mp4
    Output/
        .avi
    cognition (module)
        init__.py
        centroidtracker.py
        directioncounter.py
        trackableobject.py
    people_counter.py (driver script)
