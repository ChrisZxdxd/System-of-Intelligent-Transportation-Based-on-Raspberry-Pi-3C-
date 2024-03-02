# System-of-Intelligent-Transportation-Based-on-Raspberry-Pi

· The project uses human recognition technology to automatically detect whether a pedestrian wants to pass the crosswalk, and adaptively switches traffic lights. It also uses sensor detection technology to greatly improve the safety of large sections of curved blind spots, ensuring high traffic efficiency.

· As of December 31, 2023, this project has participated in subject competitions and won national awards. It has been approved and successfully completed at the provincial level in the College Student Innovation and Entrepreneurship Project. It has currently applied for a utility model patent and has been approved, and is still Pending publication status.

# Details of This Project
For this project, we will subdivide it into deep learning of human body recognition algorithm, learning hardware development boards such as Arduino, Raspberry Pi and Openmv, and building a cloud platform or web page to synchronously communicate the hardware status to the cloud platform. The cloud platform Perform statistics and calculations on the data.

For road sections with traffic lights, we will use deep learning algorithms to continuously train the model to improve the accuracy of human recognition and vehicle recognition. The algorithm will be implanted into the development board to run, driving the camera to automatically identify whether there are pedestrians waiting for the traffic lights, and counting the waiting times. The number of people at the traffic light and the traffic volume on the road section are uploaded to the cloud platform for analysis, and then the most appropriate time for the traffic light change to be maintained is calculated through models and algorithms. It ensures that when the traffic flow is large and the pedestrian flow is small but there are constantly pedestrians waiting for the traffic light, the green light time of the lane is lengthened to avoid unnecessary traffic congestion, relieve traffic pressure under different conditions, and flexibly adjust the traffic mechanism. When it recognizes that someone is about to cross the road, the system will automatically count down the digital tube. When the countdown ends, it will open the barrier barriers on both sides of the crosswalk and change it to a green pedestrian light. After the release is completed, the system stops identifying for a period of time to ensure smooth flow of vehicles when there is a large flow of people. The traffic flow and pedestrian flow of each road section detected by the development board driven by the camera will be uploaded to the cloud management system in real time. Traffic managers can visually observe the traffic conditions of each road section, and can remotely manually coordinate and control the change of traffic lights through the cloud platform. Or go to the field to control the traffic light system.

For curves, we will use the Arduino development board as the core, use sensors to detect in real time whether there are pedestrians or vehicles passing in the opposite lane, and use the development board to control the display and warning lights to remind drivers and pedestrians who want to make the curve.

![示例图片](https://github.com/ChrisZxdxd/System-of-Intelligent-Transportation-Based-on-Raspberry-Pi/blob/6cf55ff3d9d8ccff9736c289039d8454233b0eb4/System%20Working%20Principle.png)

As shown in ①②③ in the figure above, Raspberry Pi and Arduino cooperate with each other and control the traffic components; as shown in ④⑤⑥, Raspberry Pi can upload data to the cloud platform, which will analyze and process the data, visualize the data, and provide feedback For the Raspberry Pi, the Raspberry Pi can intelligently control traffic components based on real-time traffic data; as shown in ⑦, the Arduino that controls components such as curved ultrasonic wave and human body infrared pyroelectric can also upload data to the cloud platform, and finally Feedback to Raspberry Pi.

#No reproduction is allowed without authorization.
