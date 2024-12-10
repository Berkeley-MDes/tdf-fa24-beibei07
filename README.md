

# Table of Content
[week 1](README.md#week-1)  
[week 2](README.md#week-2)  
[week 3](README.md#week-3)   
[week 4](README.md#week-4)     
[week 5](README.md#week-5)     
[week 6](README.md#week-6)  
[week 7](README.md#week-7)  
[week 8](README.md#week-8)  
[week 9](README.md#week-9)    
[week 10](README.md#week-10)    
[week 11](README.md#week-11)   
[week 12](README.md#week-12)   
[week 13](README.md#week-13)   
---

# Week 1: 
## Week of 09/05/2024
Reflections:

This week, to prepare myself for the first project (Rhino+Grasshopper), I planned to try a beginner tutorial to design a structure using Grasshopper. I have some experience working with Rhino, but never in Grasshopper, I I speculated it to be very similar to Rhino. However, Grasshopper is nothing I have expected, the experience to me felt like linking electric wires, and I was totally lost looking at all the boxes and numbers each represent something I do not how to use. Very soon, I made a mistake by linking the exploded tree to Arc instead of Arc 3Pt, this rendered the curves generated to be 2 dimensional rather than flowing with the lofted shape I generated previous. 

![image](https://github.com/user-attachments/assets/40a8d12d-79d9-404d-b351-4cee0ab4f506)
![image](https://github.com/user-attachments/assets/874f745f-5a7c-41c5-84d4-4cb52d9e0f13)

This mistake, however, enlightned me to understand how these terms and numbers are related to the lines and shapes I used to work with. Very simply, a arc has to have three points to be established in a three dimensional space, so when I wrongly inputted the values from exploded tree to "Arc" not "Arc 3pt", the generated shape became 2D. Although the term "Arc" and "Arc 3Pt" is only the tip of an iceburg among the all terminologies Grasshopper uses, I begin to felt more confident in learning this tool. 

The Grasshopper process and final structure I generated: 
![image](https://github.com/user-attachments/assets/ac76dd7a-3856-45fe-b087-268a94b233b7)
![image](https://github.com/user-attachments/assets/a6cf5e98-de26-45e5-a0dd-49b3e66e485b)

Speculations:

Many tools today, such as Adobe AI and PS, are starting to integrate artificial intelligence to make the user experience much easier and efficient, a potential future development for Grasshopper I think is also AI integration. For example, when I am building this structure for an architecure project, AI assistant might be able to tell me its strucutural integrity, its estimate material use, etc. Or, for user's convinence, AI might be used to generate shapes and structure by inputting natural language. 

For future direction of this work, since I am very interested to learn more about Grasshopper, I think for my first project, I will try to employ as much as this tool as possible, most likely use it to design lightweight geometric structures. 


Sketches, Drawings, and Diagrams

Becasue I am very intrigued with lightweight structure and what to employ it in my first project, I looked for inspirations on Pinterest and build a moodboard/refrence board.
![image](https://github.com/user-attachments/assets/4c27c8db-82a2-4fc9-95cf-6ed59ca12c33)
And I quickly sketched a few phone stand designs inspired by these lightweight structures. Most of them are very inpractical, but just as a quick exercise to brainstorm and also practice sketching skills. 
![Image_20240905154309](https://github.com/user-attachments/assets/31b1c9b6-3dee-4ecc-aad8-ac8b500e58b1)


# Week 2: 
## Week of 09/05/2024




![image](https://github.com/user-attachments/assets/6e1f6210-d0c3-4dd5-88ac-7460d1c86033)
![image](https://github.com/user-attachments/assets/f0d81a98-3824-4617-ba6a-9614e30bff23)






Learning basic UI and features
![image](https://github.com/user-attachments/assets/fab1f7d8-263e-4039-9c83-e4f5eef66842)
Merge (so can know which data set creates the first circle and which creates the second)
Shift + drag: connect two wires to one node 
![image](https://github.com/user-attachments/assets/2ffd5df3-9e45-44c6-bfe6-2c05e678711e)
![image](https://github.com/user-attachments/assets/de732caa-edf4-4628-a611-abbed6907b71)
Parameters: empty geometry containers
Reight click point--set one point: can colate a point in Rhino file (a way to connect Rhino with Grasshopper, especially helpful when want to designate a point on a existing Rhino design)
![image](https://github.com/user-attachments/assets/69e844b4-1d82-462c-a1c4-3eed2b45149c)
Reight click point--Clear value: clear the point selected in Rhino file
![image](https://github.com/user-attachments/assets/6acd4eea-5680-4c0b-ba5e-e70c4aadc475)
![image](https://github.com/user-attachments/assets/581359b4-ec60-45e2-b905-9b629255e3db)
Reight click point--set multiple point: allow to create multiple points in Rhino file 
![image](https://github.com/user-attachments/assets/e20ff998-e75c-4b8f-a418-a5761148469f)
Reight click point--internalize data: encode the points selected in Rhino into Grasshopper (so even if Rhino file is not saved, the points still have references, but breaks the link of these points, i.e. operating the points in Rhino will not incure subsequent changes geometry created via Grasshopper). 

Parameter
![image](https://github.com/user-attachments/assets/2e3715db-b048-48da-a3c0-53e8e7fb8981)
6 types of geometry: point, curve, surface, Brep, mesh, SubD


Click + insert key: short cut to bake the geometry into the currently active layer in Rhino (cannot create group geometry, cannot select layer)


# Week 3: 
## Week of Sep. 09/12-19  
### Reflections: New Things Learned   
This week I completed my first Projet of this semester: Computational Design and learned useful technical skills in Rhino, Grasshopper, and 3D printing. I made a seed germinator using Rhino and Grasshopper, and used 3D printing to manufacture it in PLA. When exploring Grasshopper, I discovered some useful combinations of components. The work process could be quicker and easier by memoruzing and retreiving them whenever needed. Downbelow, I'll briefly analyze each of them for my future conveniences.   

#### 1. Creating a clamp   
<div align="center">
  <img src="https://github.com/user-attachments/assets/ebd5e418-abe6-4695-bd4c-b68df3449820" alt="creating clamp" width="80%"/>
</div>  
When a number slider do not satisfy the need to limit numeric value within a range (EX: the case I encountered is when the input is below a certain amount, the output radius start to increase instead of decreasing). In this case creating a clamp using Minimum and Maximum component will be helpful.  
                                                                                                            
Understand it like this: B is a filter. In the maximum setting, all values greater than B can pass through, while values smaller than B are transformed into B and then pass through. In the minimum setting, all values smaller than B can pass through, while values greater than B are transformed into B and then pass through.  
                                                                                                            
In the example: In the maximum setting, all values greater than 0 (B) can pass through, while values smaller than 0 are transformed into 0 before passing through to the minimum A value. Then, in the minimum setting, all values smaller than 2.8 (B) can pass through, while values greater than 2.8 (B) are automatically recognized as 2.8. Therefore, in this system, the values are locked within the range of 0 to 2.8.                                                                                                                                                                                                                   
#### 2. Draw Curved Line 
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/40fa789a-0c3f-4110-8d66-db63a430e3c4" alt=points and vertex" width="100%"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/2f5d4e67-12a1-4690-9e6e-128d866dff8b" alt="tangent line" width="100%"/>
    </td>
  </tr>
</table>
<div align="center">
  <img src="https://github.com/user-attachments/assets/53459c92-a54f-4f26-be42-bb7567d04dc9" alt="creating clamp" width="80%"/>
</div>  
Just like in Illustrator, Grasshopper can draw curved lines that are adjustable.    
Steps:  
                                                                                                            
1. Use Construct Point to create a point, then use Vector XYZ to control the tangent of that point. By using Vector Display Ex, the tangent is displayed as a gray arrow on the curve.    
2. Create two Merge components, inout all Construct Points into one, and all Vector XYZ into one. Make sure paired points and vector are matched in the two merges (D1 pair with D1, etc.).  
3. Create a Tangent Curve component, input Merged points into its vertices, and input Merged vectors into its tangents. Connect the Vector Display Ex into the outpit of the two merges to display the tangent.    
                                                                                                            
<div align="center">
  <img src="https://github.com/user-attachments/assets/87009edf-f5e0-45a5-af9f-fbba25d5d68a" alt="end points" width="80%"/>
</div> 
Sometimes a line is not enough, we want to create a closed shape. This can be achieved through offseting the tangent curve, extracting the end points of both curves (End Points component), and create line by using these points (Line component). Merge all the lines (Merge component), then join them using Join Curve into one continuous curve.  
                                                                                                            
#### 3. Create Grid of Points  
<div align="center">
  <img src="https://github.com/user-attachments/assets/8040f5c0-33ef-4377-8e43-70b0a24c44de" alt="end points" width="80%"/>
</div>  
To create a grod of points, first use Construct Domain to define the size/range of the grid. Input the result into the domain of two Range compoents, then connect the steps to a number slider, which can be used to control the number of points that are evenly distributed within the domain.  
                                                                                                            Currently, the grid only have a horizontal/vertical/diagonal row of points. To fill up the grid, input the result from Range compoenents into the Cross Reference compoent. Finally use Construct Point to instatiate the points.  
                                                                                                            
#### State of Work Assessment:  
What I did well: 
1. I explored many different techniques in Grasshopper to accomplish the final result I envisioned. I did not modified my design because I do not know how to do a certain manipulation, but kept the learning attitude to dive in the problems and solve them.
2. I explored the now feel comfortable to create relationships between various aspects of design, so modification can happen quickly and easily. This is what I regard as the most important aspect of computational design.
What I could improve:
1. I wish to not only explore patterning and modeling, but also leverage some physical calculation functions in Grasshopper, such as funding the center of gravity, and use them to make my design more resiliant across various situations.
                                                                                                         
### Speculations:  
<div align="center">
  <img src="https://github.com/user-attachments/assets/678b0522-e1fe-455a-8679-0b5a195ab015" alt="end points" width="80%"/>
</div>  
As AI become a popular trend, many creative work platform are utilizing this technology to create faster and easier workflow. In adobe Illustrator, users can put in command to quickly change the color of the entire illustration. Designers can use this feature to quickly gain an undertanding of color choices, which could take hours to accomplish before the AI arrival.  
                                                                                                            Grasshopper can certainly benefit from levergaing the power of AI. For example, users do not need to manually create all the components and connect them, they can simply describe what result they want (maybe AI can ask users to add some constraint for a more guided result), then AI will generate them a Grasshopper diagram they can then alter to adjust the design. Each part of the diagram could also be text descriptive, this saves users' effort in understanding the terms and features. By incoporating AI, Grasshopper could be used for the unprofessionals to create their own designs and save time for professional designers.  
                                                                                                            
### Link to the Grasshopper Project Video:
https://youtu.be/i21BiLD5xEc  
https://drive.google.com/drive/u/0/folders/1zDJGID57NZNYDydazGOXSmxJ7tzvU22K  
                                                                                                            
# Week 4
## Week Sep. 19-26
### The Digital Ecosystem
<div align="center">
  <img src="https://github.com/user-attachments/assets/2b7915ec-3908-4a09-b960-c1abda3cf59b" alt="end points" width="100%"/>
</div>  
  
Xiaomi has developed an extensive smart home ecosystem through its Mi Home platform. This system enables users to control a wide range of smart home devices through a centralized app (called Mi Home) and other connected devices. Like Amazon Alexa, Xiaomi has also developed an AI asistant named Xiaoai, by directing talking to smart speaker with Xiaoai installed, users can directly control the smart devices with their voice. This Xioami digital ecosystem has been in use at my home for several years, so I decided to talk about it for this project.    

### Refelctions  

# Week 5
## Week Sep. 26-31   

For this week's mini projects, I am using Particle Web IDE (VS code is encountering some compiling issues which I absolutely do not know how to solve, hopefully Jeff can figure it out...) and Photon 2 micorcontroller.  

### "Hello World"   
                                                                                                                                      
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/ebdf56fc-13d9-4ff5-81ef-b122bc1d5ca9" alt="Image 1" width="100%" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/4c7864a9-f20d-43d4-8939-551c3a15d1d0" alt="Image 2" width="100%" />
    </td>
  </tr>
</table>
<div align="center">
  <img src="https://github.com/user-attachments/assets/11a0ee42-2261-4d1e-aedb-9bae52711360" alt="end points" width="80%"/>
</div>  
                                                                                                                
This first mini project I worked on is to print "Hello World" in the console. After successfully printed this command, I took a closer look at the script and identified two variables that I can manipulate to adjust the behavior of the result. The first is actual text that is being printed out (e.g. "Hello World"), I changed it to "I love CAT!" for testing.   

<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/6d8c46d1-29fb-4974-92a1-ad6dfdd2823f" alt="Image 1" width="100%" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/2a1e8241-b2b2-4161-8d2f-698cdbb57a95" alt="Image 2" width="100%" />
    </td>
  </tr>
</table>    
                                                                                                             
                                                                                                  
Additionally, I manipulated with delay() function to control the rate of priting the message "I love CAT!". With a smaller number, the printing rate is faster; with a bigger number, the printing rate is slower.  
Video showing printing in console with deplay(3000): https://www.youtube.com/watch?v=iB9YzXJQ7x8
Video showing printing in console with deplay(500): https://youtu.be/raQHR2QPEGg


### "Change Periodicity" 

After successfully printed "Hello World!", I took a step further to manipulate the behavior of the printed message: introduce some randomness to the printing rate. Based on my understanding of the code Jeff has given, the randomness works in the following steps:  
<div align="center">
  <img src="https://github.com/user-attachments/assets/764ca3af-ad55-45a9-af63-3a5f6d47f887" alt="end points" width="80%"/>
</div>  
1. First, create a change_period function and then give periodicity a random range from 300-1000.  
<div align="center">
  <img src="https://github.com/user-attachments/assets/7eaa41f3-a1e3-4bd5-8dcf-62124ff5a1cd" alt="end points" width="80%"/>
</div>  
2. Then, call the function when button is being pressed.  
<div align="center">
  <img src="https://github.com/user-attachments/assets/74d43c25-5cf2-4327-855d-e02649ae6f8e" alt="end points" width="80%"/>
</div>  
3. Lastly, assign periodicity to delay. The random number from 300-1000 will be the time delayed inbetween each message printed.  
                                                                                                            
By understanding how periodicity works in the script, I can manipulate it to control the printing rate of the message. Below are some examples:    
Random (300-1000): https://youtu.be/qTnGmh6C2OY  
Random (100-300): https://youtu.be/kYl4h5hGSbs  

### "Blink Outside"
At this point I feel very intrigued by changing periodicity and introducing randomness to the system. So I choose "make it blink outside" as an exploration into how to use priodicity to manipulate perpherial devices (LED light). 
<div align="center">
  <img src="https://github.com/user-attachments/assets/4ad48045-17f0-41b2-9f17-2f94ba22d193" alt="end points" width="80%"/>
</div>  

Different from the previous minin project, this time LED light is introduced, Periodicity need to also manipulate the flashing rate of the LEDs. In the loop function, LED first turns on and last for delay(100), then turns off. If no periodicity is introduced, the loop function will immediately tuerns the LED back on by runing these aruguments again.  To change this, by calling the change-period function when button is being pressed and adding delay(periodicity), LED lights will delay for a random length before turning back on. 
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/761f9afd-fe59-45c2-832e-e8373824bf15" alt="Image 1" width="100%" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/8e54895f-3c5f-4468-a425-907bcfd1a4ad" alt="Image 2" width="100%" />
    </td>
  </tr>
</table>  
                                                                                                             
After manipulating with the randomness, I could obtain different flashing rate of the LED lights. Here are some examples:  
Random (300-1000): https://youtu.be/_19pnoKgRdo  
Random (100-400): https://youtu.be/rorzfNyxSd0  

### "Button Led Pulse"  

# Week 6

## Reflections
This week, I focused on integrating and prototyping with hardware components, specifically a Stemma QT interface board, Photon 2, and an APDS 9960 proximity/gesture/color sensor. My first task involved soldering the Stemma QT interface board, which was crucial for establishing stable connections between the Photon 2 and the sensor. Through this process, I gained practical experience with soldering techniques, learning how to ensure reliable electrical connections for communication between the components.

In terms of prototypes, I created three functional setups:

### 1. Proximity Sensor Prototype
By programming the APDS 9960, I configured it to detect hand proximity and print numerical values to the console when my hand approached the sensor. This provided immediate feedback, allowing me to fine-tune the threshold values and better understand the sensor's sensitivity.

<div align="center">
  <img src="https://github.com/user-attachments/assets/56e05225-b523-4215-a80f-7c071d3605e1" alt="Proximity Sensor Prototype" width="100%"/>
</div>

Video URL: https://youtube.com/shorts/6-ypDB4BNUQ

### 2. Gesture Sensor Prototype
Building on the proximity setup, I programmed the sensor to recognize hand gestures. It could differentiate hand positioning (left, right, far, near), which provided insight into gesture recognition algorithms and enhanced my understanding of real-world applications for proximity sensors in user interface design.

### 3. Proximity-Controlled LED
I combined the proximity sensor and an LED circuit (using a breadboard and jump wires) to create a responsive light setup. When my hand approached the sensor, the LED illuminated. This project solidified my knowledge of wiring and circuit design and demonstrated how proximity sensing could directly influence other components in a circuit.

<div align="center">
  <img src="https://github.com/user-attachments/assets/8c106c2a-9388-465a-b13f-67c4e2aa8b35" alt="Proximity-Controlled LED" width="100%"/>
</div>

Video URL: https://youtube.com/shorts/AsEia1FgLRQ

Each prototype worked successfully, and seeing the immediate, physical responses to my interactions was satisfying. I feel that my soldering skills and familiarity with interfacing sensors have improved significantly, and I am gaining confidence in my ability to troubleshoot minor hardware issues.

## Speculations
In the near future, I believe tools like the Photon 2 and Stemma QT will continue to grow in their adaptability and ease of use, especially with more sensors and modules becoming compatible. The rapid development of plug-and-play hardware components suggests a future where even complex sensors and actuators can be seamlessly integrated into prototypes without much manual setup, allowing designers and developers to focus more on creative applications rather than technical connections.

For my own work, I see potential in expanding these prototypes into more interactive applications. For instance, I could create a gesture-controlled interface where hand motions influence multiple elements, such as a series of lights or a display that reacts to different gestures. Additionally, I could explore using the APDS 9960's color detection capabilities to further enhance user interaction, perhaps creating responsive environments that change lighting or visuals based on detected colors. This progression would not only deepen my understanding of sensors but also open doors to more sophisticated interaction designs, aligning well with my focus in experiential and storytelling design.


# Week 7

## Reflections
This week, my team and I concentrated on developing and formalizing our project idea for the **Particle Photon 2-Based Calendar ball -- Rememberall**. Our objective is to design a context-aware interactive orb that visually represents Google Calendar events through dynamic lighting and sensor-based interactions. By integrating the Particle Photon 2 microcontroller with various sensors, LEDs, and cloud services, we aim to create a physical device that can sync with a user’s Google Calendar, displaying events through color changes and sensor responses. This would offer an intuitive, hands-free way to keep track of upcoming events and reminders.

### Key Aspects of the Project Proposal
1. **Hardware Components and Integration**: 
   - We plan to use the Particle Photon 2 board for its cloud connectivity and processing capabilities, paired with an RGB LED to display colors corresponding to event status.
   - A gyroscope/accelerometer sensor will detect user interactions like shaking the rememberall. For instance, if an event is approaching, shaking the rememberall might trigger it to glow orange. If no events are near, it could turn green, providing immediate visual feedback.
   - Additional components, such as buttons, a photoelectric sensor, and vibration motors, may be added to enhance interactivity and feedback.

2. **System Architecture and Process Design**:
   - We sketched an initial system architecture, outlining the connections between components: the Photon 2, STEMMA QT sensors, Google Calendar API, RGB LEDs, and cloud services.
   - A process flow diagram was also created to map the end-to-end data flow. This begins with collecting sensor input and ends with triggering specific lighting effects based on the user’s calendar events.
   - This design stage helped us understand how data from Google Calendar would move from the API to the Photon 2 device, and how different inputs would be processed to control the LEDs and vibration motor.
  <div align="center">
  <img src="https://github.com/user-attachments/assets/27e25f99-3a5e-46c0-b26b-7c7c0812b4b2" alt="System Architecture Diagram" width="100%"/>
</div>

 <div align="center">
  <img src="https://github.com/user-attachments/assets/0f53a560-3955-4c4a-82e2-2e7456d6bb1a" alt="System Architecture Diagram" width="100%"/>
</div>

3. **Experiments and Testing Plan**:
   - We outlined a series of experiments to test each component individually and as part of an integrated system. 
     - For instance, I am responsible for validating the connection between Google Calendar and the Photon 2, which involves setting up API calls and ensuring that event data can be reliably fetched and displayed on the rememberall.
     - My teammates are focused on experimenting with the LED light responses triggered by motion detection and testing the low-power sleep mode on the Photon 2 to improve energy efficiency.
   - Each test is designed to identify integration challenges and refine our prototyping methods. This approach allows us to tackle potential issues early in the project, ensuring that each component can work harmoniously within the overall system.

### My Role and Contributions
My primary focus this week was on the API integration aspect of the project. I researched how to connect the Google Calendar API to the Particle Photon 2, examining the best practices for making HTTP requests and processing the responses on the Photon. Through this, I learned a lot about handling API responses in real-time and configuring the Photon 2 to sync with external cloud data. I also familiarized myself with Particle’s cloud service tools, which will be crucial for managing the data flow between Google Calendar and our physical device. This setup will allow us to map calendar events to specific colors on the rememberall, making the device both visually engaging and functional.

Overall, this week laid a strong foundation for the technical and logistical aspects of our project. We clarified our objectives, distributed roles, and identified areas that may require further iteration. I feel that the project is on track, and I am more confident in our ability to tackle the API challenges and hardware integration as we move forward.

## Speculations
As we progress, I anticipate that our primary technical challenge will be ensuring seamless communication between the Particle Photon 2 and the Google Calendar API, especially when dealing with real-time data updates and response times. Currently, the IoT field is evolving rapidly, with cloud providers enhancing their support for real-time and low-latency applications. I believe that in the near future, cloud-connected IoT devices like ours will benefit from even more efficient API handling and improved latency, making such integrations faster and more stable. This trend will allow us to create more interactive and responsive devices with real-world applications in productivity and time management.

For the **rememberall**, I envision expanding its capabilities beyond basic calendar integration. The device could potentially become a multi-functional personal assistant, syncing with various data sources, such as reminders, weather updates, or even health data, to provide relevant information through visual cues. Additionally, incorporating machine learning algorithms could allow the rememberall to learn user behaviors, adjusting its responses based on recurring patterns in the calendar. This would further personalize the user experience, making the rememberall a truly adaptive and context-aware device.

Our immediate future direction will focus on building and testing each component, gradually integrating them into a cohesive prototype. I believe that with the advancements in IoT and cloud technologies, this project has the potential to evolve into a practical product for smart home or office environments, enabling users to visualize and interact with their digital schedules in a tangible, engaging way.

# Week 8

## Reflections
This week, I made significant progress on the API integration for our **Rememberall** project, focusing on setting up a system to retrieve Google Calendar data through Particle Cloud and Google Cloud services. Initially, I struggled with direct API integration and couldn’t get the event data to display on the Photon console. After getting help form my classmate Tommy, I learned about using a **Webhook** as an intermediary between **Particle Cloud** and **Google Cloud Run Function**, which ultimately enabled the successful retrieval of Google Calendar data.

### Key Components and Process Overview
1. **Google Calendar API**: This API provides access to event data from Google Calendar, which is necessary for our project’s context-aware functionality. By querying this API, I can pull event start and end times to drive the visual responses of the rememberall.
   
2. **Google Cloud Run Function**: To control the flow of data, I implemented a custom Cloud Run function that receives HTTP requests from the webhook, queries the Google Calendar API, and filters out unnecessary information. It extracts only essential data, such as start and end times, formats it into a JSON response, and sends it back to the webhook. This function is designed to operate in UTC, ensuring that the events are time-accurate.

3. **Webhook**: Serving as a bridge, the webhook listens for event triggers from the Photon 2 via Particle Cloud, initiates a request to the Cloud Run function, and forwards the response back to the Photon. This intermediary step was crucial for establishing reliable communication between Particle Cloud and Google Calendar API, as the Photon 2 does not natively support direct API calls.

To initiate the process, I programmed the Photon 2 to publish a private event (`Particle.publish("get_calendar_events", PRIVATE)`) to Particle Cloud. This publication activates the webhook, which listens for this event. Upon receiving it, the webhook sends an HTTP request to the Google Cloud Run function, fetching the event data from Google Calendar in JSON format. After parsing this data, it sends it back to Particle Cloud, where the Photon 2 can access it and control the LED based on event timing.

<div align="center">
  <img src="https://github.com/user-attachments/assets/dcf28f21-8f71-490c-b867-4c55eef24248" alt="System Architecture Diagram for Particle Cloud and Google Calendar API Integration" width="100%"/>
</div>

### Prototype Demonstration and Photon Code
In the Photon 2 script, I configured the device to subscribe to the webhook responses from Particle Cloud. This allows it to listen for JSON data returned from Google Calendar. Here’s an overview of the key functions in the code:
- **JSON Parsing**: Using the `ArduinoJson` library, I parse the JSON response to extract the start and end times for events.
- **Time Conversion and Synchronization**: One challenge I encountered was synchronizing the Photon 2's time zone with the Google Calendar event data’s time zone. Initially, I tried converting both the Photon 2’s internal clock and the event data to local time, but this approach proved cumbersome. I realized that the Photon 2 syncs its system time with the Particle Cloud’s NTP server, defaulting to UTC, just like the Google Calendar API. This alignment eliminated the need for manual time zone conversions. However, despite both being in UTC, the formats differ—Photon uses Unix timestamps, while the API uses ISO 8601 strings. I implemented a `parseISO8601()` function to convert ISO 8601 to Unix timestamps, ensuring accurate time comparisons for LED responses.
- **Event Status Check**: By comparing the current time with event start and end times, the Photon determines the event’s status. If an event is ongoing, it prints “Event is ongoing” and lights up the LED in red. If the event is upcoming, it lights up in blue; if there’s no event, it turns green.

<div align="center">
  <img src="https://github.com/user-attachments/assets/6d68063b-8207-42e3-8cea-bc541e6eca5a" alt="Photon 2 Code for JSON Parsing and Event Time Comparison" width="100%"/>
</div>

This coding exercise helped me gain a deeper understanding of JSON handling on embedded devices, time synchronization, and time-based control. The Photon now accurately updates the LED based on the Google Calendar event status, achieving a key milestone in our project.

### Webhook Logs and Debugging
The webhook logs display the entire sequence, from the Photon’s event publication to the HTTP request and response cycle with Google Cloud Run Function. By reviewing these logs, I was able to verify the data exchange, monitor any delays, and ensure that the expected data was received. This debugging process was instrumental in refining our integration.

### Google Cloud Run Function Code
In Google Cloud Run, I wrote a JavaScript function to handle incoming webhook requests, query Google Calendar API, and return only relevant event data. The function excludes unnecessary fields (like event creator) and formats the response to include only start and end times. By focusing the response data, I minimized bandwidth and processing requirements on the Photon 2.

<div align="center">
  <img src="https://github.com/user-attachments/assets/f024aeb7-ed98-4139-af36-e2133f35acb7" alt="Google Cloud Run Function Code for Event Filtering" width="100%"/>
</div>

## Speculations
I anticipate that the use of webhooks and cloud functions will become increasingly prevalent in IoT integrations, as they enable devices to connect to complex APIs and handle large datasets effectively. This project taught me the importance of cloud bridging services to overcome hardware limitations, and I foresee these types of integrations becoming standard in IoT development.

For our project’s future, we can expand the orb’s functionalities to include more sophisticated interactions. For example, we could adjust the LED behavior based on event importance, using different colors or patterns to indicate high-priority events. We might also integrate other services, such as weather or task management, to create a more comprehensive interactive display. This would transform the orb into a multi-purpose notification device, aligning with smart home trends that prioritize visual feedback and contextual information.

# Week 9

## Reflections
This week, completed my second project of the semester, the **Rememberall** and learned useful technical skills especially in getting API reponses. My contributions were focused on the product’s physical design, integration testing, and final demonstration recording.

### 1. Product Modeling and Manufacturing
Using **Rhino**, I modeled the Remembrall in four distinct parts:
- The upper hemisphere
- The lower hemisphere
- The box that houses the microcontroller inside the sphere
- The lid for the microcontroller box

After completing the model, I moved on to manufacturing the parts using 3D printing. I used **PLA for the lower hemisphere** due to its durability and **translucent resin for the upper hemisphere**. The resin’s translucency allows the LED light to shine through, creating a visually engaging effect that aligns with our design goals. Additionally, the slight flexibility of the resin helps improve tolerance when fitting the two hemispheres together.

<div align="center">
  <img src="https://github.com/user-attachments/assets/a8b0b3af-ffc0-41b8-9e1c-57500ef664d8" alt="Rhino Model of Remembrall" width="100%"/>
</div>

<div align="center">
  <img src="https://github.com/user-attachments/assets/3b3953ee-6056-4163-a605-05881cb843c3" alt="Rhino Model of Remembrall" width="100%"/>
</div>

### 2. Hardware and API Integration Testing
My teammates and I worked together to integrate the hardware code with the API response. This involved thoroughly testing the device’s response to Google Calendar events by adding, modifying, and deleting events in real-time. Each test allowed us to evaluate the functionality and responsiveness of the Remembrall, ensuring that it correctly updated based on event statuses:
- **LED color changes** to indicate event statuses (e.g., upcoming, ongoing, or no events).
- **Event timing adjustments** to test synchronization between the API response and hardware.

This collaborative effort not only helped us refine the integration but also provided a chance to debug issues in real-time and enhance the user experience.

<div align="center">
  <img src="https://github.com/user-attachments/assets/8eee9808-5873-4916-b07f-fdcb86fc85c2" alt="Hardware and API Testing" width="100%"/>
</div>

### 3. Final Demonstration Video
To document our progress and showcase the final prototype, we recorded a video demonstration of the Remembrall in action. This video highlights the different stages of functionality, from initial setup to real-time response to calendar events. Working on this video provided a holistic view of our accomplishments and helped us visually communicate the concept and capabilities of the Remembrall.

<div align="center">
  <img src="https://github.com/user-attachments/assets/831387ed-c58f-48b4-a825-5bea273c5d3b" alt="Hardware and API Testing" width="100%"/>
</div>
Video URL: https://youtu.be/lZJBR3rfQgQ

## Speculations
As we move toward the project’s completion, I can envision additional enhancements to improve both the design and functionality of the Remembrall. For instance, we could experiment with other materials that offer better light diffusion, or add modular components to extend its functionality (e.g., sound alerts for high-priority events). Additionally, as IoT technology advances, future iterations of the Remembrall could integrate multiple data sources, making it a multifunctional tool for managing not just schedules, but also tasks, reminders, and other notifications.

Our testing phase also revealed the potential of real-time data integration and the impact it can have on interactive devices. In future projects, I hope to apply these insights to create even more responsive and user-centered designs.

# Week 10
# Week of 11/09/2024

## Reflections
This week, I shifted my focus to developing a large language model (LLM) for my Project 3. Using a website called **ZeroWidth**, I learned how to construct an LLM tailored to act as an agent that represents myself (Vivian) and assists with navigating my TDF projects. This exploration gave me valuable insight into various components of LLM development and customization, helping me better understand the nuances of building a functional and responsive agent.

### Experiments
1. **Experiment 1**
<div align="center">
  <img src="https://github.com/user-attachments/assets/7f852b0d-6da4-4125-af6f-ef2426e39fba" alt="ZeroWidth Platform with LLM Components" width="100%"/>
</div>
In this experiment, I experimented with adjusting the temperature setting, which affects the style and depth of the LLM’s responses:
Temperature 1.6   
1. Produces a more elaborate and conversational response.  
2. Adds background information about Rhino and Grasshopper’s use in fields like architecture and design.  
3. Feels detailed and engaging but can be more verbose.  
Temperature 1   
1. Yields a concise, straightforward answer.  
2. Focuses on the core question without extra elaboration.  
3. Suitable for users who prefer direct, factual responses.  
The difference in response shows that a higher temperatures encourage richer, more exploratory responses, while lower temperatures lead to more focused and precise answers. 
1. **Experiment 1**
 
2. **Experiment 2**:
  <div align="center">
  <img src="https://github.com/user-attachments/assets/9245e6ec-4a53-46af-82a4-35804dc2cc3e" alt="ZeroWidth Platform with LLM Components" width="100%"/>
</div> 
In this experiment, I tested how changing the instruction in the prompt affects the LLM’s response. I focused on two types of changes: adding extra information and altering the tone. Because I do not have a knowledge base for the LLM to retrieve information by now, to add extra information, I simply instructed the LLM to include a joke at the end of each response. The LLM successfully performed this task. For altering the tone, I asked the LLM to use a "cowboy personality." This shifted the response style significantly, introducing playful, Western-themed language like “Howdy, partner!” while keeping the core information. This experiment shows the usefulness of modifying the instructions, it could help easier retrieval of intended information without needing to ask for it every time; it can also make the interaction more engaging and personalized. 

3. **Experiment 3**:
<div align="center">
  <img src="https://github.com/user-attachments/assets/7cf92e25-8d46-4e66-ba4a-ecebb6fd2972" alt="ZeroWidth Platform with LLM Components" width="100%"/>
</div> 

<div align="center">
  <img src="https://github.com/user-attachments/assets/631790a6-a9f0-4139-b2fa-5e7dd5639320" alt="ZeroWidth Platform with LLM Components" width="100%"/>
</div> 
In this experiment, I observed the impact of knowledge base design, specifically chunking, on the accuracy of responses.
Background: This semester in my TDF course, I worked on three main projects: computational design, Photon 2 (Remembrall), and an LLM system.
Initially, I set up my knowledge base with a token size of 300, resulting in 29 chunks. Using this setup, the LLM response included errors, misidentifying small experiments as full projects and failing to accurately recognize the actual number of projects. But it has included a link to my experiment outcome and project files. 
To improve accuracy, I restructured my knowledge base with a smaller token size of 150, creating 62 chunks. This adjustment allowed the LLM to generate more precise responses, correctly identifying the three main projects and providing accurate descriptions for each. But this time, the LLM did not provide me URL to my project file. 
From this experiment I learned:
Chunking Strategy: Dividing information into chunks allows the LLM to search and retrieve relevant sections of knowledge more effectively. Smaller chunks tend to make retrieval more precise because the model can access specific pieces of information without irrelevant details. Larger chunks provide more context (e.g., project file URL) but may include extra information that isn't directly relevant, potentially diluting the response.
Number of Tokens per Chunk: The token limit within each chunk also impacts retrieval and response quality. Fewer tokens (e.g., 150) make each chunk smaller and more focused, allowing the model to pinpoint specific details quickly. This is useful for detailed, specific queries. However, larger token limits (e.g., 300) may give the model more context to work with (provide project file URL). 

4. **Experiment 4**:
<div align="center">
  <img src="https://github.com/user-attachments/assets/2c16800f-bacd-474a-9db6-58a1d4268663" alt="ZeroWidth Platform with LLM Components" width="100%"/>
</div> 
In this experiment, I attempted to create variables to guide the LLM toward providing more specific answers. I created a variable with the key ${LEARNING} and a default value of "Rhino." By applying this variable, the LLM was supposed to filter the knowledge base and retrieve information more relevant to "Rhino," ideally focusing on the computational design project (used Rhino). However, I discovered that since Rhino was mentioned sporadically across many projects without concentrated emphasis, the LLM often generated inaccurate responses, randomly selecting projects rather than focusing on the one that truly centered on Rhino.
To improve accuracy, I changed the variable value to terms that were more frequently and intensively mentioned, specifically "LLM" and "Photon 2." With these values, the LLM was able to provide more accurate responses regarding the relevant projects. This indicates that for the variable to effectively guide responses, its value should be a prominent component in the knowledge base, with a strong association to specific chunks of information. In other words, the variable value needs to be closely linked to a distinct, well-defined topic within the knowledge base to ensure the LLM retrieves accurate, relevant responses.

## Speculations
Looking forward, I see potential in enhancing this LLM’s capabilities to better understand and interact with my TDF projects. With further refinement, I could train the agent to offer not only navigation assistance but also project-related insights, recommendations, or reflections. As ZeroWidth evolves, I expect even more advanced options for fine-tuning and training models, which could lead to greater personalization and contextual awareness.

Developing this LLM has also sparked ideas for broader applications. In future projects, I might experiment with using similar agents to assist with other areas of work, such as research management or task tracking. This project has shown me the potential of LLMs as adaptive and interactive tools, aligning well with my interest in system and service design.

# Week 11
# Week of 11/07/2024-11/14/2024
## Video Link: https://youtu.be/FDk4oq9VinU

## Reflections
This week, I focused on creating a **project video** to showcase my LLM project, which I have been developing using the ZeroWidth platform. The video highlights the functionality of the LLM I built, including its role as an agent that represents me (Vivian) and assists in navigating my TDF projects. The process of crafting this video required a combination of technical explanation, storytelling, and effective visuals to communicate the purpose and capabilities of the LLM.

### Video Creation Process
1. **Scripting**: I started by drafting a script to structure the video. This included an introduction to the LLM project, its objectives, and the key features I implemented (e.g., agent representation, knowledge base, and customizable settings like temperature). Writing the script helped me focus on the most important aspects of the project to share.

2. **Recording**: I captured video clips demonstrating how the LLM interacts with queries and navigates TDF projects. These clips showcased the seamless integration of components like the knowledge base and the agent's ability to handle project-specific inputs effectively.

3. **Editing**: To bring the video together, I edited the recordings, adding transitions, annotations, and voiceovers to ensure clarity and engagement. This process taught me a lot about organizing technical content into a visually appealing and understandable format for an audience.

4. **Finalizing**: The final video combines narration, screen recordings, and overlays that clearly explain how the LLM works, its applications, and its potential future enhancements. I feel that the video effectively demonstrates the project’s scope and functionality.

<div align="center">
  <img src="https://github.com/user-attachments/assets/341c7050-43e2-4b03-952e-df712144c65f" alt="Screenshot of Project Video" width="100%"/>
</div>

Creating this video not only helped document my work but also provided me with valuable experience in visual communication and storytelling. The process reinforced the importance of presenting technical content in a way that’s accessible and engaging to a broader audience.

## Speculations
As I worked on editing the video, I began to reflect on the potential of **AI in video editing**. AI-powered tools are already transforming video production, offering features like automated scene selection, intelligent cropping, and real-time transcription. In the future, I anticipate AI will play an even larger role in video editing, enabling:
- **Personalized Editing Styles**: AI could learn a user's editing preferences over time, automatically applying consistent styles, transitions, and effects across multiple projects.
- **Content-Aware Editing**: Advanced AI systems could analyze video content, identify the key moments or themes, and suggest or even automate edits based on the context.
- **Speech and Emotion Recognition**: AI could enhance storytelling by syncing visual effects or music with the tone of voice or detected emotions in a video.
- **Automated Accessibility Features**: Real-time generation of captions, translations, and alternative formats could make videos more accessible to diverse audiences.

These advancements would significantly streamline video production workflows, making high-quality editing accessible to more people. For my future projects, I’m particularly interested in exploring AI tools to enhance visual storytelling and integrate interactivity into project demonstrations.

This week’s experience has reinforced my belief in the synergy between AI and creative processes, and I’m excited to see how these technologies will continue to evolve.

# Week 12
# Week of 11/14/2024-11/21/2024

## Reflections
This week, I focused on two primary areas for our **final project**: experimenting with **storytelling integration** using Inky in Unity for the front-end game and exploring materials for the **physical product**, which includes a neck-wearable device.

### 1. Storytelling Integration in Unity
I began experimenting with **Inky**, a tool for creating interactive storytelling, and integrating its output into Unity to power the narrative for the game portion of the project. The goal was to create a dynamic, engaging storytelling experience that adapts based on player interactions. Key aspects of this experimentation included:
- **Ink Script Development**: I used Inky to craft branching storylines that align with the game’s objectives. These scripts incorporate decision-making elements, allowing players to influence the story's direction.
- **Unity Integration**: By importing Ink scripts into Unity, I worked on connecting the game mechanics to the narrative. This required scripting interactions so that player actions trigger specific story branches, ensuring a seamless blend between gameplay and storytelling.
- **Challenges and Refinement**: The main challenge was synchronizing Unity's game state with the Ink script’s variables. I spent time debugging to ensure the game correctly reflects story changes and provides smooth transitions between narrative and gameplay.

This experimentation laid the groundwork for the game’s front-end storytelling and helped me understand the technicalities of combining interactive narratives with Unity’s framework.

<div align="center">
  <img src="https://github.com/user-attachments/assets/9f943f41-e731-438d-ba23-bd9046f71030" alt="Inky Integration in Unity" width="100%"/>
</div>

### 2. Physical Product Experimentation
On the hardware side, I explored materials and sensors to create a **neck-wearable device** for data collection. This device will be part of the project’s physical product and aims to measure neck movement using flex sensors. Here’s what I worked on:
- **Flex Sensor Integration**: I tested flex sensors as the primary input mechanism for capturing neck muscle movements. The sensor’s sensitivity and response time were key factors in determining its effectiveness.
- **Material Experimentation**: I experimented with **web foam** and **fabric** to design the wearable. Web foam provided flexibility and comfort, while fabric offered durability and better adaptability to different neck sizes. I compared their performance in terms of sensor placement, stability, and user comfort.
- **Prototyping and Testing**: Combining the sensors and materials, I created initial prototypes to test how well the wearable captures data during neck movements. These experiments helped identify optimal material combinations and sensor configurations.

<div align="center">
  <img src="https://github.com/user-attachments/assets/a698dc4e-4ee1-47e1-80c4-047c43401a83" alt="Neck-Wearable Prototype with Flex Sensor" width="100%"/>
</div>
<div align="center">
  <img src="https://github.com/user-attachments/assets/784f4621-d8ae-44fb-bdac-6df90f208441" alt="Neck-Wearable Prototype with Flex Sensor" width="100%"/>
</div>
<div align="center">
  <img src="https://github.com/user-attachments/assets/69e1a1fb-42b3-4291-b365-ca27e8cd7b85" alt="Neck-Wearable Prototype with Flex Sensor" width="100%"/>
</div>


### 3. Lessons Learned
This week’s work highlighted the importance of both technical integration and physical prototyping in creating a cohesive product. While the storytelling integration is shaping the front-end experience, the physical wearable adds a meaningful layer of interaction, bridging the game with real-world data collection.

## Speculations
In future development, I envision integrating **ChatGPT into Unity** to create even more **adaptive storytelling experiences**. While Inky provides branching narratives, ChatGPT could introduce real-time, dynamic dialogue and plot generation. Here’s how I imagine this integration could evolve:
- **Real-Time Interaction**: ChatGPT could enable NPCs to respond dynamically to player input, creating conversations that feel more personalized and immersive.
- **Player-Centric Narratives**: By analyzing player behavior, ChatGPT could adapt the storyline to match individual playstyles, ensuring a unique experience for each player.
- **Content Scalability**: ChatGPT’s ability to generate text on the fly would reduce the need for pre-written scripts, allowing for more expansive worlds with endless narrative possibilities.
- **Hybrid Approach**: Combining Inky for structured story branches and ChatGPT for dynamic content could balance narrative control and player freedom, offering a richer storytelling experience.

For the physical product, future iterations could involve integrating the wearable with Unity to directly influence the game’s story or mechanics based on real-time data from the flex sensors. This would make the game more interactive and responsive to player actions, further blurring the line between the physical and digital realms.

This week’s experimentation has set the stage for integrating interactive storytelling and real-world interaction in our final project, pushing the boundaries of what’s possible with Unity and hardware integration.


# Week 13
# Week of 12/02/2024-12/05/2024

## Reflections
This week, I worked on integrating **OpenCV with Unity**, capturing and transforming digital twin movements, and constructing a **web mesh wearable model** for our final project. The focus was on bridging real-world interactions with digital representations and creating a flexible physical prototype for the wearable device.

### 1. OpenCV Integration with Unity
I began testing **OpenCV integration with Unity** to create a **digital twin** that reflects real-time user movements. The goal was to mirror the user’s physical movements within Unity by capturing motion data using OpenCV and translating it into the digital twin’s movements. This integration allowed me to:
- **Set up real-time motion tracking**: Using OpenCV, I tracked specific movements of the user and applied them to the digital twin in Unity. For example, head or neck movements were reflected immediately in the digital twin, providing a visual representation of the user's actions.
- **Debugging and Optimization**: I encountered challenges with latency and precision but worked on optimizing the motion tracking pipeline to ensure smoother real-time reflections.

<div align="center">
  <img src="https://github.com/user-attachments/assets/d2f2f4b1-17d7-40f4-a08b-2712edc0d47f" alt="OpenCV Integration with Unity for Digital Twin" width="100%"/>
</div>

### 2. Capturing and Animating the Digital Twin
Building on the real-time reflection, I explored turning the **digital twin’s movements into animations**:
- **Movement Capture**: I used OpenCV to record the digital twin’s movements and saved these as animation clips. This process allowed me to transition from real-time motion capture to reusable animations.
- **Trigger-Based Animation**: To expand functionality, I shifted the digital twin’s control from real-time reflection to **trigger-based animations**. These animations were activated using keyboard inputs, simulating pre-defined motion states.
    - For instance, pressing a key triggered the digital twin to perform a specific action (e.g., nodding or tilting).
    - This system was designed to eventually replace keyboard inputs with **data from the wearable device**, ensuring that physical interactions would directly influence the digital twin in Unity.

### 3. Constructing the Wearable Model
For the physical wearable, I used **Rhino** to design a **web mesh model** that aligns with the project’s aesthetic and functional goals. The wearable model needed to be soft and flexible to accommodate neck movements while securely housing sensors:
- **Web Mesh Design**: I created a lightweight web-like structure in Rhino, ensuring it provided enough flexibility for user comfort while maintaining structural integrity for sensor placement.
- **TPU Printing**: I printed the model using **TPU** material. TPU was chosen for its softness, elasticity, and durability, which made it ideal for wearable applications. The resulting prototype offered the necessary flexibility to adapt to various neck sizes and movements.

<div align="center">
  <img src="https://github.com/user-attachments/assets/f96208e1-95c2-4dba-af35-57b57edaee35" alt="Web Mesh Wearable Model Designed in Rhino" width="100%"/>
</div>

### 4. Lessons Learned
This week’s work demonstrated the potential for combining digital and physical elements in interactive systems:
- OpenCV’s real-time tracking capabilities provided a solid foundation for creating digital twins that respond to physical movements.
- Transitioning from real-time tracking to trigger-based animations helped me better understand Unity’s animation system and how external inputs can control pre-defined animations.
- The success of the TPU-printed wearable confirmed that the material choice and design approach could meet the project’s functional and aesthetic requirements.

## Speculations
Looking ahead, I see significant potential for expanding the integration of **OpenCV and Unity**. Real-time digital twins could evolve into fully interactive avatars, enabling applications in gaming, virtual reality, and remote collaboration. By replacing keyboard triggers with data from the wearable device, we could create a seamless interaction loop between physical inputs and digital outputs, offering a more immersive experience.

On the hardware side, the web mesh wearable could be refined further to incorporate additional sensors or feedback mechanisms (e.g., vibration motors or LEDs) to enhance interactivity. The use of TPU also opens possibilities for exploring other flexible materials, such as silicone, to optimize comfort and durability.

This week’s experiments have laid a strong foundation for connecting the physical and digital components of the project, pushing the boundaries of interactivity and personalization.











                                                                                                            
                                                                                                        

                                                                                                          













                                                                                                            
                                                                                                      




