BBox-Label-Tool
===============

A simple tool for labeling object bounding boxes in images, implemented with Python Tkinter.

**Updates:** 
- 2017.5.21 Check out the ```multi-class``` branch for a multi-class version implemented by @jxgu1016

**Screenshot:**
![Label Tool](./screenshot.png)

Data Organization
-----------------
LabelTool  
|  
|--main.py   *# source code for the tool*  
|  
|--Images/   *# directory containing the images to be labeled*
|  
|--Labels/   *# directory for the labeling results*
|  
|--Examples/  *# directory for the example bboxes*

Dependency
----------
python 3
pillow
python3-tk

Startup
-------
$ python main.py

Usage
-----
**0. The current tool requires that .JPEG images to be labeled reside in /Images/001, /Images/002, etc. You will need to modify the code if you want to label images elsewhere.**
**0b. Each category/directory of images needs its own examples or you will need to modify the code if you don't have examples for each category.
1. Input a number (e.g, 1, 2, 5...), and click 'Load'. The images along with a few example results will be loaded.
2. To create a new bounding box, left-click to select the first vertex. Moving the mouse to draw a rectangle, and left-click again to select the second vertex.
  - To cancel the bounding box while drawing, just press <Esc>.
  - To delete a existing bounding box, select it from the listbox, and click 'Delete'.
  - To delete all existing bounding boxes in the image, simply click 'ClearAll'.
3. After finishing one image, click 'Next' to advance. Likewise, click 'Prev' to reverse. Or, input the index and click 'Go' to navigate to an arbitrary image.
  - The labeling result will be saved if and only if the 'Next' button is clicked.

Credits
-------
This repo was originally created by [puzzledqs/BBox-Label-Tool](https://github.com/puzzledqs/BBox-Label-Tool).
