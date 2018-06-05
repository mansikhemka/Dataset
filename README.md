# Dataset
Indian Transport


Steps to generate labels:


(1) Rename all the images: Retain only the numeral ID of image and discard the first part of the string.
(On mac OS X, this can be done by selecting all the files of the folder simultaneously, pressing right click and then select rename)

(2) All images must be in the .jpg format (Case sensitive). It can again be done using rename.

(3) Save all the images in BBox-Label-Tool-Multi-Class/Images/001/

(4) Install the following dependencies to run the script:

    For Python3 : tkinter, PIL 

    On Ubuntu run : sudo apt-get install python3-tk
    
                    sudo python3 -m pip install pillow

 Run main.py in BBox-Label-Tool-Multi-Class 

    On terminal : python main.py

(5) An interface appears. Type 001 in the text field on top and press Load. The first images appears.

(6) Before labeling bbox, choose the 'Current Class' in the Combobox and make sure you click 'ComfirmClass' button. I have given an index to each of our class as follows:

0: Bus

1: Private car

2: Auto-rickshaw

3: Two-wheeler

4: truck

5: Pedestrian

6: Bicycle

7: Taxi


(7)To create a new bounding box, left-click to select the first vertex. Moving the mouse to draw a rectangle, and left-click again to select the second vertex.

To cancel the bounding box while drawing, just press .
To delete a existing bounding box, select it from the listbox, and click 'Delete'.
To delete all existing bounding boxes in the image, simply click 'ClearAll'.

(9) After finishing one image, click 'Next' to advance. Likewise, click 'Prev' to reverse. Or, input the index and click 'Go' to navigate to an arbitrary image.

(10) The labeling result will be saved if and only if the 'Next' button is clicked.

(11) The images get stored in BBox-Label-Tool-Multi-Class/Labels/001/





Converting custom format to YOLOv2:

(1) Save all the images in labels/images/

(2) Save all the label files generated in the first part in labels/input/

(3) Run custom_to_yolo.py

