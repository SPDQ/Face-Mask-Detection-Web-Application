# Face-Mask detection web application with load balancer
This project is an assignment for Cloud Computing course. The project contains a user application and manager application. Both application are written in Python Flask and deployed on AWS EC2.
<br>
### User application
In the user application, each user can upload an image and the app will detect faces and masks in that images. The application has log in panel and stores the history of uploaded images. There is an administer account that can add or delete user. The user guide can be found in doc/user_app_doc.pdf.
<br>
<img src="https://github.com/SPDQ/ECE1779_A2/blob/master/doc/userapp_home.png" height="250px" width="400px">
<img src="https://github.com/SPDQ/Face-Mask-Detection-Web-Application/blob/master/doc/user_detect.png" height="250px" width="400px">
<br>
### Manager application
This application is developed for a manager to control the amount of resources offered to user app. We call the instance running user app worker. In the manager application, the manager can add or delete workers. The user guide can be found in doc/manager_app_doc.pdf. 
<br>
<br>
In the homepage of manager app, there is a list of all the workers with their detail.
<br>
<img src="https://github.com/SPDQ/Face-Mask-Detection-Web-Application/blob/master/doc/manager_list.png" height="300px" width="600px">
<br>
<br>
The application can also monitor the CPU utilization and HTTP requests of each worker. 
<br>
<img src="https://github.com/SPDQ/ECE1779_A2/blob/master/doc/manager_cpu.png" height="400px" width="600px">
<br>
<br>
The number of healthy workers in past 30 minutes is also shown in the application. 
<br>
<img src="https://github.com/SPDQ/ECE1779_A2/blob/master/doc/manager_wknum.png" height="400px" width="600px">
<br>
<br>
The application has the function of auto-scaling. The configuration of auto-scaler can be set by manager. 
<br>
<img src="https://github.com/SPDQ/ECE1779_A2/blob/master/doc/auto_scaler_config.png" height="320px" width="600px">
<br>
