

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
## Week of 09/12-19  
### New Things Learned  
When exploring Grasshopper, I discovered some useful combinations of components. The work process could be quicker and easier by memoruzing and retreiving them whenever needed. Downbelow, I'll briefly analyze each of them for my future conveniences.   

#### 1. Creating a clamp   
<div align="center">
  <img src="https://github.com/user-attachments/assets/ebd5e418-abe6-4695-bd4c-b68df3449820" alt="creating clamp" width="80%"/>
</div>  
When a number slider do not satisfy the need to limit numeric value within a range (EX: the case I encountered is when the input is below a certain amount, the output radius start to increase instead of decreasing). In this case creating a clamp using Minimum and Maximum component will be helpful.  
                                                                                                            
Understand it like this: B is a filter. In the maximum setting, all values greater than B can pass through, while values smaller than B are transformed into B and then pass through. In the minimum setting, all values smaller than B can pass through, while values greater than B are transformed into B and then pass through.  
                                                                                                            
In the example: In the maximum setting, all values greater than 0 (B) can pass through, while values smaller than 0 are transformed into 0 before passing through to the minimum A value. Then, in the minimum setting, all values smaller than 2.8 (B) can pass through, while values greater than 2.8 (B) are automatically recognized as 2.8. Therefore, in this system, the values are locked within the range of 0 to 2.8.                                                                                                                                                                                                                   
### 2. Draw Curved Line 
<table>
  <tr>
    <td>
      <img src="https://github.com/user-attachments/assets/40fa789a-0c3f-4110-8d66-db63a430e3c4" alt=points and vertex" width="50%"/>
    </td>
    <td>
      <img src="https://github.com/user-attachments/assets/2f5d4e67-12a1-4690-9e6e-128d866dff8b" alt="tangent line" width="50%"/>
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
                                                                                                            
### 3. Create Grid of Points  
<div align="center">
  <img src="https://github.com/user-attachments/assets/8040f5c0-33ef-4377-8e43-70b0a24c44de" alt="end points" width="80%"/>
</div>  
To create a grod of points, first use Construct Domain to define the size/range of the grid. Input the result into the domain of two Range compoents, then connect the steps to a number slider, which can be used to control the number of points that are evenly distributed within the domain.  
                                                                                                            Currently, the grid only have a horizontal/vertical/diagonal row of points. To fill up the grid, input the result from Range compoenents into the Cross Reference compoent. Finally use Construct Point to instatiate the points.   












Jiahua (Vivian) Zhu
The Seed Sprouter
https://youtu.be/i21BiLD5xEc









































Project Challenge Level Rationale 

The project challenge level I chose is 03-Axolotl, this is because this project poses some challenges to me since I have barely used grasshopper before. However, I want to take this challenge to deepen my understanding in the elusive concept of computational design and reach my goals of 1) feel comfortable in using Grasshopper 2) explore the capability of computational design and its basic logic to be able to apply it in enforcing my future design processes. 

System Diagrammatic Analysis 

One fascinating aspect of computational design is its flexibility in adapting to different user’s needs in various use cases. With this in mind, I included various adjustable features in the seed sprouter design which I will further demonstrate below with the AEIOU framework and diagrammatic analysis of the Grasshopper diagram. 

First Iteration

The first iteration of the design is focusing on the use case of needing the seed sprouter to be compatible with different vase shapes. 

Activities: Users use a seed sprouter 
mainly to grow seeds/ leftover vegetable scrap into sprouts. To achieve this goal, users engage in a series of activities: they soak seeds (may not be performed depending on the seed type), place them in the sprouter, make sure seed sprouter is in contact with water in the vase, fill in water if not enough, and monitor growth. Users perform these activities so they can 1) harvest the sprouts as spices / cooking ingredients 2) observe growth for joy, which leads to subsequent activities such as harvesting or observing, causing diverging design goals. 

Environment: The seed sprouter is most likely to be placed in the kitchen environment, often in small or confined spaces like countertops or window sills. To facilitate growth, direct contact with sunlight will be desirable. Seed sprouter design needs to fit small spaces and be made of lighter materials to avoid excessive heat absorption and the material needs to be water and mold resistant since it is used in moist environment. Aesthetic-wise, users with either expectation (cooking or observation) would prefer the seed sprouter to blend well with the kitchen environment, so choosing a aesthetically neutral design style would be desirable. 

Interaction: Upon first use, users would need to find compatible vases so the seed sprouter would fit in. Next, users should fill water into the vase to a point the seed is partially soaked. Users are expected to frequently observe the water level and fill water periodically by lifting the seed sprouter up and pouring water into the vase or directly pouring on the sprout depending on the sprout's type and growth status. If users’ goal is in harvesting the plant, they would occasionally trim off part of the sprout when in need. 

Objectives：The objectives involved are mainly the seed sprouter itself and the vase it sits on. The seed sprouter should be made of material that is reusable, durable, and non-toxic. Based on previously analyzed interactions and activities, sprouter needs to be 1) compatible with a variety of vase shapes 2) can be handled easily / ergonomically fitting most users’ hands 3) sits on vases steadily to avoid tipping when the sprout is being rimmed 4) make sure water level is easily observable. 

Users: For a simple seed sprouter design, users are unlikely professional gardeners, they are more likely to be amateur hobbyists who like to observe plant growth and without spending too much time on gardening; and/or health-conscious individuals who are interested in growing fresh sprouts at home. For these users, the sprouter’s design should be convenient, easy to use, easy to accommodate the given condition at home.

From the AEIOU analysis, a few points stand out. In summary, the seed sprouter design requirements are: 1) easy to handle and sits steadily on top of vases, 2) be able to accommodate various vase shapes users have, 3) moist-resistant materials, and 4) made in a lighter color to avoid excessive heat absorption. In order to comprehend computational design’s ability of modifying model to accommodate different circumstances, I adopted a well designed sprouter found online and used it as the basis to explore the second design requirement (vase accommodation. Material decisions will be covered in other sections. 

My Grasshopper diagram consists of four main parts: 1) constructing the vase, 2) building relationship between z positions of the vase and the sprouter 3) building relationship between radius of the vase and the sprouter 4)constructing the sprouter. 



For the first part of constructing the vase, I identified four necessary features in building a vase of any shape, which are top edge, neck, belly, and base; then I introduced two types of input, z-position and radius, to make four circles representing these four features. By manipulating these features, the vase can be transformed into any desired shape. Then by lofting and offsetting, a vase with wall thickness is built. 

The seed sprouter can be constructed in the same way by first identifying some key features, making circles that represent them, lofting, and offsetting. The difference is that the z-position and radius of the sprouter need to be built in relationship with the vase, so that when the vase is being modified, the sprouter could change along to ensure consistent fitness. The features identified are top edge, belly (where the seeds are being placed), and bottom edge. One additional circle is being added near the top edge feature as shape control when lofting. 



For building the Z-position and radius of the sprouters, I applied mathematic calculations in Grasshopper (subtraction, addition, multiplication, and division),  used the radius and Z-position of the vase’s top edge as one of the input and other numbers on the slider as the other. The results define the basic profile of the sprouter. 

Since part of the sprouter extends inside the vase, and the sprouter itself is also modifiable for customization, I need to make sure that when it is being modified, the sprouter will never collide with the vase. In order to do this, I created a “filter” using Minimum, Maximum, and Domain components to manually clamp the radius input within a range. By combining this “filter” with another Division component, I make sure that the radius at the sprouter's belly (its widest part) will remain at least 1.5 times smaller than the neck of the bottle. 



After defining the relationship and constraints, I lofted the circles to make one surface of the sprouter and used offset to build the other surface. Then I extracted both top and bottom edges of the two surfaces and lofted them to obtain the necessary surfaces to make an enclosed shape. Finally, by merging the four surfaces, the seed sprouter is built. 

Second Iteration 

After completing the first iteration, I contemplated my 	need as a seed sprouter user, adding on one more design requirement: adaptation to various seeds, not just avocado. This challenge me to use Grasshopper to control the number and radius of perforations on the sprouter. 



My first attempt is to use the model built from the first iteration as the basis, and Boolean Difference it with cylinders to make perforations. However, although I used Brep Join to merge the four surfaces, Grasshopper is still not recognizing the model as a solid shape, which prevents it from performing Boolean Difference. Therefore, I decided to use Revolution as an alternative path to build the basic sprouter’s shape. 



The first step to build the sprouter using revolution is to construct the profile line drawing. I created three line segments using the Tangent Line component, joined and offset them to obtain a line on the other side. Then by extracting the end points of both line segments and inputting them into the Construct Line, I obtain the short segment between these two lines. Finally by merging them, I have a closed profile line drawing. The next step is to revolve. I reoriented the profile drawing to match the axis and target plane I have constructed early on, and by using the Revolution component, a closed shape sprouter is being generated. 



The next step is to build a grid of points that defines the location and number of the perforations. I first used Construct Domain and Range components to create a row of points, and then used the Cross Reference component to extend the row into a matrix and points. The range and number of points are modifiable by manipulating the input. At this step, the matrix is in a square shape, not matching the circular shape of the sprouter. To achieve a circular matrix, I first generated a circle by intersecting a plane with the sprouter and performed the Brep | Plane component; then I used the Distance component to calculate the distance between each point on the grid and the circle’s center; finally, by using the Smaller Than component, I identified points that have a distance from the center points larger than the circle’s radius, which means they lay outside of the circle. By culling these points, the matrix is trimmed into a circular shape. 



Now the points are constructed, I need to make sure the circles generated from them will have an inverse relationship between their number (of circles) and radius. This ensures that when the number of perforation increases, they will not overlap each other. This is achieved by building a calculation system using List Length, Multiplication, and Division components. 



Finally, by extruding these circles and Boolean Differenced them with the Sprouter, the final model is generated. The number of perforation can be manipulated by the number of steps in the Range component constructing the matrix; and the size of perforation can be adjusted within the calculation system. 

Fabrication Analysis 

Material decision is another important aspect in this seed sprouter design. As analyzed using the AEIOU framework, the material needs to be 1)moist-resistant materials, and 2) made in a lighter color to avoid excessive heat absorption. Leveraging the technique and material available to me, I choose 3D printing as my fabrication method. For material, I explored both PLA and resin, both were able to give me lightweight, moist-resistant, and light-colored results. Resin produces a significantly finer result with prolonged fabrication time, for environmental friendly and power saving purposes, PLA might be a preferable choice. Production time could also be controlled by manipulating the offset distance to change to wall thickness. 


Prototype Demonstration 



Project Challenge Result 

To explore computational technologies, I focused primarily on developing techniques that build constraints and relationships between different parts of the design. This approach ensures that when one element is modified, the other components adjust accordingly, maintaining the overall integrity of the design and eliminating the need for the designer to manually adjust each element for fit. By automating these relationships, I was able to streamline the design process, making it more efficient and reducing the potential for errors during iterations. These experiments not only allowed me to better understand the role of computational tools in design but also taught me to observe the key features of objects and how they interact with one another. This perspective helped me recognize the importance of flexibility and adaptability in design, as I began to comprehend how different elements could be manipulated to meet diverse user needs and function effectively across various environmental conditions. Moreover, this approach emphasizes the importance of scalability, ensuring that the design can evolve smoothly without compromising its usability or performance, even when faced with unforeseen challenges or changes in user behavior.

Speculation

Human Experiences:

As computational design tools become increasingly integrated into the design process, human experiences with everyday objects, like a seed sprouter, will shift dramatically. In the context of the Anthropogenic Environment—where human activities are the dominant influence on the environment—the expectations for how objects interact with our surroundings may evolve. Users will likely expect products that are not only functional but also responsive and adaptable to changing conditions. For instance, in the case of a seed sprouter, users may expect the design to automatically adapt to varying humidity levels or daylight conditions, optimizing sprouting processes without manual intervention. Culturally, there may be a stronger expectation for designs that blend seamlessly into different lifestyles and contexts, driven by the desire for sustainability and efficiency. The boundaries between design, function, and environment will blur, and cultural expectations might prioritize objects that actively participate in environmental sustainability and self-regulation. In this sense, the seed sprouter may no longer be seen as a passive tool but as an active participant in human-environment interactions.

Engineering

In terms of engineering, computational design tools and systems thinking will push the boundaries of how products are made and customized. Rather than designing objects with fixed parameters, future designs might be more modular and capable of self-adjustment based on real-time user feedback or environmental data. This could shift cultural expectations towards products that are not only mass-produced but also personalized to the user’s individual preferences and the specific environments they inhabit. For example, the seed sprouter could be designed to adjust automatically based on the types of seeds being grown, the user's geographic location, or the amount of available light, without requiring manual adjustment. The use of computational design in engineering might also shift expectations toward a more sustainable approach, where materials and manufacturing methods are optimized for minimal waste. In this way, products like the seed sprouter could be designed with built-in recyclability, biodegradability, or repurposability in mind, aligning with growing cultural concerns about environmental impact.

AI

AI will play a pivotal role in shaping systems of Observe > Measure > Model > Evaluate > Fabricate > Test, particularly by making these systems more interconnected and autonomous. In the case of the seed sprouter, AI could be employed to observe and measure environmental conditions—such as temperature, humidity, and light—and then model the optimal conditions for seed growth based on this data. AI-driven systems could continuously evaluate the sprouting process, adjusting variables like water levels or air circulation automatically. This kind of dynamic feedback loop would reduce the need for human intervention and ensure that the system is always operating at peak efficiency. AI could also enhance the fabrication process by offering more precise, data-driven insights into material selection, design modifications, and optimization techniques, leading to more sustainable and effective product outcomes. 


Peer Feedback Response

Categorization of Feedback

Desire for Demonstration and Application: Many respondents expressed interest in seeing a live demonstration or real-world application of the design, such as using an avocado, green onion, or other real-world objects to test how the design interacts with physical items.

Iteration Process and Parameter Adjustability: The feedback frequently mentioned the success of the iterative process, including the ability to adjust parameters for different contexts 

Interest in Surface Perforation and Patterning: A few respondents noted that it would be interesting to see further development in specific aspects, such as surface perforation and patterning.

Suggestions for Improvement in the Presentation: While most responses were positive, some suggested minor improvements, such as shortening the explanation or including more visual demonstrations of the product in use.

Analysis of Feedback

Strengths: The strongest feedback centered on my ability to clearly communicate and explain the computational design process, even when working with complex Grasshopper functions. Respondents found the explanations approachable and appreciated the modular nature of the design. These comments indicate that my design process resonated well with the audience, particularly in terms of clarity and the usefulness of the iterative methods.

Opportunities for Improvement: The desire for a physical or video demonstration of the product’s interaction with real-world objects, such as an avocado or green onion, highlights the audience’s interest in seeing how the design functions beyond the digital environment. Additionally, there’s curiosity about expanding the design to include surface perforation, indicating that more exploration in this area could further elevate the design.

Suggestions for Future Work: Feedback suggests that I could show more versions of the design process to illustrate how different iterations led to the final outcome. This shows a desire for a more thorough narrative of the design journey, which would help the audience fully appreciate the complexity and evolution of the design. A couple of respondents also suggested a faster explanation, which indicates that streamlining future presentations could improve engagement.

Response to Feedback and Next Steps

Enhance Demonstration with Real-World Examples: Many respondents expressed interest in seeing the design interact with real-world objects. Moving forward, I could create a video demonstration where the seed sprouter design is tested with physical items like an avocado or green onion. This will not only bring the design to life but also give the audience a clearer sense of how it performs in practice.

Further Exploration of Surface Patterning and Perforation: Given the interest in surface perforation, I could explore adding this feature in future iterations. This exploration can include how perforation affects airflow, water drainage, and overall aesthetics. By incorporating patterning options, I can also add a layer of personalization that aligns with user preferences for different styles.

Streamline Presentation for Efficiency: While the majority of the audience found the explanations clear, I recognize the suggestion to shorten the explanation portion. For future presentations, I can streamline my delivery by focusing on the most critical points and utilizing visual aids or storytelling techniques to ensure the process remains engaging and to-the-point.

Showcase Iteration Process More Thoroughly: Several respondents valued the iterative process but suggested showing more stages to better understand the design evolution. In response, I can include more visual examples of each stage in the process for future presentations. This will help communicate the design’s adaptability to different contexts, further highlighting its versatility.

Highlight the Computational Design System: Feedback showed strong appreciation for how I handled the complex computational system using Grasshopper. To build on this, I can continue refining the parameter-driven system, ensuring that it remains easy for users to manipulate without needing detailed knowledge of computational design. This will help users feel confident in the system’s flexibility, even if they are not familiar with the underlying technology.

Conclusion

In this report, I explored the potential and challenges of computational design through the development of a seed sprouter, a project that leveraged Grasshopper to integrate adaptability and customization in response to varying user needs and environmental conditions. The feedback from peers underscored the success in explaining complex processes clearly and highlighted areas for future enhancements such as real-world demonstrations and further exploration of design features like surface patterning. Moving forward, the plan is to refine these areas, enhance demonstrations with tangible, real-world applications, and continue leveraging computational tools to make the design process as intuitive and flexible as possible. The journey of this project not only advanced my proficiency with computational design but also enriched my understanding of its implications for sustainable and user-centered design practices. This exploration sets a firm foundation for future projects where the integration of design, function, and user adaptability will continue to evolve, meeting the dynamic demands of the modern world.

















# Github Background Information & Context
If you’re new to GitHub, you can think of this as a shared file space (like a Google Drive folder, or a like a USB drive that’s hosted online.) 

This is your space to store project files, videos, PDFs, notes, images, etc., and (hopefully, neatly) organize so it's easy for viewers (and you!) to navigate. That said, it’s super easy for you to share any file or folder with us (your TDF instructional team) - just send us the link!  As a start, feel free to simply add images to the `/assets` folder, which is located [here](/assets). 

The specific file that I’m typing into right now is the **README.md** for this repo. 
##### (💡 TIP: The .md indicates that we’re using [Markdown formatting.](https://www.markdownguide.org/cheat-sheet/)) #####
<h6> (💡 TIP 2: GitHub Markdown supports <a href="https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2"> <em>HTML formatting</em> too, including emojis 😄</a>, in case that helps!) </h6>

### :star: Whatever you write in your **README.md** will show up on the “front page” of your GitHub repo. This is where we’ll be looking for your [weekly progress reports](https://github.com/Berkeley-MDes/24f-desinv-202/wiki/3.0-Weekly-Submissions#weekly-progress-report). They might look something like this: ###

# Week 1: Example Report 1 #
## Week of 09/05/2024

This week, I designed a cool phone stand made of rocks. Check out all my cool sketches and progress photos from this week below, etc., etc....

<img width="200" alt="Cool Phone Stand made of rocks" src="assets/exampleimg.png">

---

It's time to start making this space your own! If you want to save these instructions, make a copy.  Also, feel empowered to delete everything in this README.md and start documenting! 

Excited to work with you,
your TDF teaching team

PS: let us know if you have any questions!!

PPS: 

## Quick Links, compiled here for your convenience: ##

- [TDF Wiki](https://github.com/Berkeley-MDes/24f-desinv-202/wiki) - the ultimate source for truth and information about the course and assignments
- [Google Drive Folder](https://drive.google.com/drive/u/0/folders/1DJ1b6sSDwHXX6NRcQYt10ivyQSgU0ND6) - slides and other resources
- [bCourses](https://bcourses.berkeley.edu/courses/1537533) - where the grading happens
