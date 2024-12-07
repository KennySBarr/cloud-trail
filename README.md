<p align="center">
       
![AWS_logo_new](https://github.com/user-attachments/assets/a7a389ae-0c58-4096-afdf-d0586aaa44e3)

   

</p>

<h1>AWS CloudWatch </h1>
AWS (Amazon Web Services) is a comprehensive and widely adopted cloud platform that offers a variety of on-demand computing services, storage, networking, and analytics, enabling businesses to scale and innovate with flexibility and efficiency.

<h2>Requirements</h2>

- Computer with Internet Connection
- Credit Card (Required for free AWS credits)

<h2>Configuration Steps</h2>


<h3>Step 1: Search for CloudWatch</h3>

- Search in the search bar "CloudWatch" 
- Select Cloud Watch
  
![Screenshot 2024-12-07 062459](https://github.com/user-attachments/assets/bd413149-f6a6-40d3-ad5e-80f44dfc4f3a)


- Follow the prompt to the " Create Alarm" 
     - In this screenshot I already created my alarm
    
![Screenshot 2024-12-07 065241](https://github.com/user-attachments/assets/6597c4fe-8727-417f-88df-d8d890e01326)




<h3>Step 2: Search for EC2 Metrics </h3>

 - In this example the metric I chose was "EC2" metrics which will allow me to monitor things like CPU utilization, Memory Usage etc,.

![Screenshot 2024-12-07 062820](https://github.com/user-attachments/assets/5605ece4-ba84-47e1-b5c5-a8e4c94505ba)


<h3>Step 3: Click a metric to monitor </h3>

- Choose "CPU Utilization" or a metric you would want to monitor

![Screenshot 2024-12-07 062830](https://github.com/user-attachments/assets/9b4d0dd8-83fa-4451-98eb-d574c5a11a90)

<h3>Step 4: Configure your alarm </h3>

- During this step I set my configurations to send a notification through SNS to the "Root" user if the CPU utilization exceeds 70% within the first 5 minutes

![Screenshot 2024-12-07 062924](https://github.com/user-attachments/assets/828c0632-ee97-4de1-955d-d518c5346c73)

![Screenshot 2024-12-07 063033](https://github.com/user-attachments/assets/995eca96-be36-4327-948a-9f7fa4da2a0c)




- Set a rule that if it does exceed 70 percent to stop the instance from running along with a notifcation
- An incident report will also be automated as well once the alarm is set off using AWS policies
  
![Screenshot 2024-12-07 063058](https://github.com/user-attachments/assets/e696d728-57bb-4ec2-b7ca-18ef1808d50d)


![Screenshot 2024-12-07 063109](https://github.com/user-attachments/assets/88971dd7-9f92-4829-9b21-452d0805502d)


- In your alarm tab you should then see your alarm enabled with your configurations 

![image](https://github.com/user-attachments/assets/d740d83d-c1d9-4c39-a5f9-80c557fdae69)



