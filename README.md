#Real_Time_Object_Detection_using_Detectron2

<img width="430" alt="detectron2-logo" src="https://user-images.githubusercontent.com/77112134/130313040-7ba519c1-81f9-4ec0-a5e8-80394657ed32.png">

Detectron2 is Facebook AI Research's next generation library that provides state-of-the-art detection and segmentation algorithms. It is the successor of Detectron and maskrcnn-benchmark. It supports a number of computer vision research projects and production applications in Facebook.



https://user-images.githubusercontent.com/77112134/130313585-7166f7d9-afce-4c97-87b1-05866dbf653a.mp4

# Getting Started
### >>Problem Satatement

Dataset link: https://drive.google.com/file/d/1NKLt3_lPDIxGyiQ_m0QXTVygeC4V7TK7/view?usp=sharing

Dataset information: There are two folders within the dataset provided
1. test_videos - Contain videos on which your model needs to be tested

2. train - This dataset contains “Images” folder - which has images containing bat and ball. There is a CSV file “bat_ball.csv” which contains following columns “class (label)” “X axis (Top Left X-coordinate of the image )” “Y Axis (Top Left Y-coordinate of the image)” “width(width of the class (bat or ball))” , “height (height of the class (bat or ball))” , “name (Name of the image)”, “image_width”, “image_height”

1) We have to detect and localize ball and bat In a given frame. 

2) Information about the training dataset provided is as follows

  3.1 )There is a folder named “images” which has all the images containing bat and ball. These images are already annotated and the annotation file is a CSV file named “bat_ball” at the same level as the “images folder”

 3.2) the columns of the CSV file are described above

4) once We train the models test them on the videos given in the “test_videos” folder.

5) outcome - detect bat and ball in each frame of test videos and draw a rectangular bounding box around bat and ball in each frame.

>> Approach
 We approached the problem statement  in two phases.
1.we converted given dataset in one of the standard object detection dataset formats like COCO, PASAL-VOC etc. Doing this made my dataset compatible with lot of open source algorithms and frameworks. We chose COCO format as it involved much more complexities in implementation.
2.We converted existing dataset to coco format.(>>Coco json Data.ipynb)
3.


