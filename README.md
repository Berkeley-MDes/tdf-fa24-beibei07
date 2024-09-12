

# Table of Content
[week 1](README.md#week-1)

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
