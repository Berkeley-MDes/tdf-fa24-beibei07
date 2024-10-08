

# Table of Content
[week 1](README.md#week-1)  
[week 2](README.md#week-2)  
[week 3](README.md#week-3)  
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
When exploring Grasshopper, I discovered some useful combinations of components. The work process could be quicker and easier by memoruzing and retreiving them whenever needed. Downbelow, I'll briefly analyze each of them for my future conveniences.   

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
### Monday Homework  

For this week's mini projects, I am using Particle Web IDE (VS code is encountering some compiling issues which I absolutely do not know how to solve, hopefully Jeff can figure it out...) and Photon 2 micorcontroller.  
                                                                                                                                      
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
      <img src="https://github.com/user-attachments/assets/ebdf56fc-13d9-4ff5-81ef-b122bc1d5ca9" alt="Image 1" width="100%" />
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/6d8c46d1-29fb-4974-92a1-ad6dfdd2823f" alt="Image 2" width="100%" />
    </td>
  </tr>
</table>
<div align="center">
  <img src="https://github.com/user-attachments/assets/6065c7cb-93d7-4f64-85c5-cd9667cd3529="end points" width="80%"/>
</div>  
                                                                                                             
                                                                                                            
Additionally, I manipulated with delay() function to control the rate of priting the message "I love CAT!". With a smaller number, the printing rate is faster; with a bigger number, the printing rate is slower.  
Video showing printing in console with deplay(3000): https://www.youtube.com/watch?v=iB9YzXJQ7x8
Video showing printing in console with deplay(500): https://youtu.be/raQHR2QPEGg











                                                                                                            
                                                                                                      




