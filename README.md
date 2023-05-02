<h1>Object Segmentation using Mask RCNN and Yolov8</h1>

<p>This project is aimed at performing object segmentation using two popular models: Mask RCNN and Yolov8. We will be taking photos of robotics arm in the environment, annotating them on Roboflow for segmentation, and then training the two models. Finally, we will evaluate the models based on mean Average Precision (mAP), speed, and size.</p>
<h2>Step 1: Collecting Data</h2>
<p>We collected over 100 images of four robotics arm. Here are some examples of the images:</p>
<p><img src="imgs/original.jpg" alt="Image 1">
<img src="imgs/original (1).jpg" alt="Image 2"></p>
<h2>Step 2: Annotating on Roboflow</h2>
<p>Next, we annotated the images on Roboflow for segmentation. Here's a screenshot of the annotated images on Roboflow:</p>
<p><img src="imgs/robo.png" alt="Roboflow Annotation"></p>
<h2>Step 3: Training Mask RCNN</h2>
<p>We used detectron2 to train the Mask RCNN model. The code for training can be found in this Colab notebook: 
<a href="https://colab.research.google.com/drive/1-iKrwiKwUQYtPXPWe1Xo2s1-hyRI4nPU?usp=sharing" target="_new">Colab Notebook for Mask RCNN</a>.</p><p>Here's a screenshot of the training process:</p>
<p><img src="imgs/train_detectron.png" alt="Mask RCNN Training"></p>
<h2>Step 4: Training Yolov8</h2>
<p>We trained Yolov8. The code for training can be found in this Colab notebook: 
<a href="https://colab.research.google.com/drive/1iJX_n7GUFjU0J_P15wVpz2d37zZhwT7A?usp=sharing" target="_new">Colab Notebook for Yolov8</a>.</p>
<p>Here's a screenshot of the training process:</p>
<p><img src="imgs/train_yolo.png" alt="Yolov8 Training"></p>
<h2>Step 5: Evaluating the Models</h2>
<p>Finally, we evaluated both models based on mAP, speed, and size. Here are the results:</p>
<table><thead><tr><th>Model</th><th>mAP</th><th>Speed</th><th>Size</th><th>train T</th></tr></thead>
     <tbody><tr><td>Mask RCNN</td><td>0.646</td><td>20 ms</td><td> </td><td>15:30 M</td></tr>
         <tr><td>Yolov8</td><td>0.777</td><td>40.1ms</td><td>27241964</td><td>0.349 H</td></tr></tbody></table>

<h2>Step 6: Testing the Models</h2>
<h3>Detectron2</h3>
<p><img src="imgs/download11.png" alt="Image 1">
<img src="imgs/download22.png" alt="Image 2"></p>


<h3>YOLOv8</h3>
<p><img src="imgs/download1.jpeg" alt="Image 1">
<img src="imgs/download 1(1).jpeg" alt="Image 2"></p>


<h2>References</h2>
<ul><li><a href="https://github.com/facebookresearch/detectron2" target="_new">Detectron2</a></li>
<li><a href="https://github.com/ultralytics/ultralytics" target="_new">Yolov8</a></li></ul></div>
