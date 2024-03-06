# safety_equipment_tracking_yolov8
## Ultralytics Yolov8 object detection and tracking to detect, track and monitor safety equipment status

This project has been developed to showcase the potential usage of object detection and object tracking, customized to monitor events by keeping track of the time and raising a signal when a certain condition is met. It can be further customized for different scenarios and different conditions.

Object detector used: Yolov8.1.24 from Ultralytics 

The script for the helmet tracker can be found in helmet_tracker.py

There are different ways of detecting helmet removal, including training a model that differentiates humans with and without helmets. In this case, I used an approach where the algorithm checks if the helmet center location is moved away a certain distance (pixels) from the top center of the worker class (head of the worker). Note that this is probably not an ideal approach and was implemented to showcase the time monitoring of removal. The reason this may not be the ideal case is becasue people may work in various forms; standing, laying, crouched, crouched and tilted towards or away from the camera etc. or the helmet might be dropped on a surface where it does not satisfy removal distance criteria due to the camera angle. Again, the objective here was to show how conditions can be incorporated with the tracking algorithm to achieve an automatic detection and warning system. 

