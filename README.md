Here are the step-by-step instructions

##### 1- For Training : 
So used Google Colab(T4) to train our Insect Yolo model . Here we researched with various model but we got best result on Yolov8m (Insect-Yolo). In 200 epoch we got the best result. Here we Used 
Batch size = 16. 
Learing rate was = 1e-2
Optimizer = AdamW
Pool = Max
Momentum = 0.937

We from here we got our best.pt file as our trained file. 


##### 2 - Real-Time System :
We build a real-time system for our research to implement our best.pt (our trained model). 

##### 2.1 - Backend :
To developed backend of our real-time system we utilized Flask 3.1.0 . All about of backend is code is displayed in app.py in the folder structure. 


##### 3 - Frontend : 
To depeloped our real-time system's frontend we used html and for desining our website we used tailwind css. We used a background image here. 
![Insect-Detection](static/background3.jpg)


##### 4 - Predicted Output Using Our Real-time System : 
We save all of our prediction screen shot of our real-time systems in Predicted_images folder.
![Insect-Detection](Predicted_images/output1.jpg)
![Insect-Detection](Predicted_images/output3.jpg)
![Insect-Detection](Predicted_images/output4.jpg)
![Insect-Detection](Predicted_images/output5.jpg)
![Insect-Detection](Predicted_images/output6.jpg)


##### 5 - Detecting Non Insect Using Our Real-time System : 
We also check our model perfomance using image that do not contains insect.
 And our model can detect the image that don't contains any insect  and it display a message to input valid insect image. 
![Insect-Detection](Not-insect-images/notinsect-1.png)
![Insect-Detection](Not-insect-images/notinsect-2.png) 

#### Download yolov8m weights:
Download yolov8m weigths and place in your Flask app code directory.

####  Run the Python Script:
Once you're in the directory containing your app.py file, run the following command:
<b>python app.py </b>

Following these steps should launch your Flask web application, allowing you to access it through a web browser or any other HTTP client.

