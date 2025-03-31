# Development Commentary Template

## Project Outline
- ~~At Death We Part is a 2.5D platformer with light and dark mechanics to help the player progress in the story. There is two characters one who has light powers and can only stand in light, and the other who has dark powers and can only stand in darkness.~~ 

- At Death we part is a 2.5D Platformer that utalises light and dark mechanics to help the player progress through the level. The character will have two states; A light state and a dark state, this allows the player to pass through the shadow areas whislt in the dark state and the light areas whist in the dark state. This then allows the player to stand on platforms of the oppisite state (Light character can stand on the dark areas and vise versa).

- My inital goal is to create a functional swapping mechanic for the player that I can then add to by adding powers to the different states and the making puzzles around that. Then after that is completed I will then add more mechanics and polish to the game.    

- The most immediate challange I may face is making the light mechanic work and only light up the part of the platform it is touching. Another issue may be miscommunication from teammembers.  

## Research

### Methodology  
- Identify relevant sources for the project, including articles, documentation, talks, and games.  
- Detail how these sources have informed your practical work and influenced your approach.

### Game Sources  
- Ori and the Blind Forest:
Ori is a 2.5 Platformer game where the main character 'Ori' traverses through the world gaining powerups as he goes. I found the 2.5D artstyle to look very interesting with this almost storybook looking artstyle.
Find Sources that talk about oris gameplay mechanics.

- Inside:
Inside is a 2.5D game where the player must travel though a bleak empty world to using the environment to put together the story and figure out the characters objective.
Find Sources that talk about insides gameplay mechanics.

- Fireboy & Watergirl:
Fireboy & Watergirl is a 2D coop game where two players play as fireboy and watergirl, they must work together to pass the levels and avoid falling into the other characters liquid or the green goo.
Find Sources that talk about Fireboy & watergirl's gameplay mechanics.

- Little Nightmares 
Little Nightmares is a 2.5D horror game where the main character 'Six'
- Conduct research on games that are relevant to your project. Provide a brief description of each game and the insights it offers.  
- Analyse the game's approach, cross-referencing it with other sources such as articles or talks to support your analysis.  
- Explain how these insights apply to your project and influence your decision-making process.

### Academic Sources  
- Research academic papers, books, or articles that provide theoretical guidance for your project. Include a brief summary of each source.  
- Describe how the academic research applies to your project and shapes your design and development decisions.

### Documentation Sources  
## Camera Mechanic
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZmIzHtglnMM?si=jhqRReVfk8Fhn_sV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/O7SjrIrY_io?si=xUh4iTc1JVeLD4Mm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## 2D Movement
<iframe width="560" height="315" src="https://www.youtube.com/embed/0f1_qSXbqAI?si=NKyjGC-tFWcnW6Yd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Cursor Mechanic
<iframe width="560" height="315" src="https://www.youtube.com/embed/8VZtDdKApeM?si=ow2RlVm7CmGLkJtF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
- Investigate relevant documentation, tutorials, or instructional videos that provide technical insights into your tasks. Summarise the content and its relevance to your project.  
- Explain how this technical knowledge supports your project work and guides your decision-making process.

## Implementation
# Camera Mechanic

- For the Camera Mechanic I want the camera to be on a static spline, when the player leaves the room the camera will fly to the next room.
-![image](https://github.com/user-attachments/assets/685477d2-3b9f-4bc2-ab77-65d83dccc652)
![image](https://github.com/user-attachments/assets/5b969e1e-b0e8-49c0-9ba4-1785cb8c729f)
// add videos at home // 

- I fixed the way the camera was facing but now I need to make it so the camera is segmented.

- Spline Movement BP:
<iframe src="https://blueprintue.com/render/d6-zmgms/" scrolling="no" allowfullscreen></iframe>

- I wasn't a fan of how this looked so I used the Residant Evil camera system as a reference and implemented it into the game.



<video controls src="Resident Evil Style Camera Test.mp4" title="Title"></video>


- I didnt like how the camera moved so I disabled the movement and made the camera completly static.

<video controls src="Static Cam.mp4" title="Title"></video>
# 2D Movement

- I decided to remake the third person character template with my own 2D one.
- I created this using the paper ZD plugin to create 2D characters faster and more easily.
<!-- This is good, you should research this plugin in your research section. -->
- Added Paper ZD https://www.fab.com/listings/6664e3b5-e376-47aa-a0dd-f7bbbd5b93c0 // Fix Citation //
- Made the Player_BP
- I then made a PaperZDCharacter class.
 - Added Animation Source 
- Added PaperZD AnimBP
- Imported the textures and converted them into sprites
 - I turned all of the sprites into flipbooks to allow me to animate them.

 <!-- waaay to many images, you only need maybe a gif of the character moving around, or being animated in paperzd -->

 ### Animation Preview
<video controls src="Early Walking Anim.mp4" title="// add GIF //"></video>

- I Added the new sprite to the Player_BP
- To make the lighting more releastic I added cast shadow in the details tab, this will make the lighting look more realistic on the character.
- To ensure that this works in the matarials I added a MaskedLitSpriteMaterial so that the light works on the character correctly.
![alt text](image-12.png)
### Process
- Provide a step-by-step breakdown of your development process, including key milestones and decisions made throughout the project.  
- Highlight any tools, frameworks, or techniques used, and explain how they contributed to the implementation.  
- Include screenshots, diagrams, or code snippets where relevant to showcase your progress.


## Flash Light System

- I was looking into creating a 2D flashlight for the game but I was unsure how to impliment it so I looked at copilot to help me learn about how to create it.
![alt text](image-14.png)
![alt text](image-15.png)

- After tweaking the flashlight I managed to make it work correctly when the player turns left.
<video controls src="Working Flashlight.mp4" title="Title"></video>

## Flickering Light System
- for a simple puzzle idea I created a light that toggles every 3 seconds. //put vid here//

## Cursor mechanic
- To make the game feel more stylisied I added a custom cursor to the game, this step was easy but I am eventually going to make the cursor change when clicked to be more visual.
![alt text](<image copy.png>)

## Animated shadow texture 
- I animated a simple animation for the shadow platforms. I requested for the shadow to look more like squiggles, this helps the game to look more like a picture book that had been drawn into.

- I used Copilot to give me an idea of how to smoothly cycle between the frames so it looks like the squiggles are moving rather than switching in between frames.
![alt text](<image copy 2.png>)

### New Approaches  

## Light System
Due to time constraints and being repeatedly let down by my designer I had to remake the entire game idea from scratch whilst trying to keep the overall theme of loss and acceptence in tact. Instead of having 5 levels there will now be one giant level with 3 sections (attic, bedroom, basement) and the movement controls and mechanics have been simplified indefinitely or when we meet schecule deadlines. This change was unfortunate as I wanted to trust the designers reassurance that he would get everything done on time, however, they never delivered. I have also diminished the designers rights and I am now acting as lead designer and I have stationed the old designer to doing backround assets and sound design.

## Camera System
- originally the player camera was going to be static and fly to the next room when the player walked into it, However, I found the spline to be finicky so I gave the camera a more standard look. If I have some spare time I will look into creating it again. But for now the camera works as intended. 
- Detail any innovative or new approaches you explored during the project.  
- Explain why these approaches were chosen and how they differ from standard practices.  
- Evaluate the success of these approaches, including any challenges faced and lessons learned.

## 2 player system

- I have scrapped the 2 player system and instead I have one sprite followed by a small ghost to give the same effect

### Testing
- Document the user testing conducted, specifying the type of tests used (e.g., automated testing, guided user testing, blind testing).  
- Present feedback or issues identified during testing, using graphs, tables, or visual aids to summarise results.  
- Describe how these issues were addressed. If any issues were not resolved, provide a clear justification for leaving them unaddressed.

## Technical Difficulties
<!-- Here is where you need to specify any issues your encountered and how you fixed or didnt fix them. its ok not to be able to fix things, you can justify why you didnt fix, maybe time, maybe its noticable, etc. -->
## Camera System

- The camera is not looking at the correct location, cannot rotate camera
- Identify any technical difficulties encountered during the implementation phase.  
- I was having an issue of being able to turn the camera even though the game was in 2D making the movement controls weird. This was a simple fix I just added the mouse onto the screen all the time to disable camera movement. It is also set up for the power mechanics which will need the mouse to operate.

<iframe src="https://blueprintue.com/render/d6-zmgms/" scrolling="no" allowfullscreen></iframe>

- Provide details on how these issues were diagnosed and resolved.  
- If any difficulties remain unresolved, explain the impact on the project and any mitigation strategies used to minimise their effect.  
- Reflect on what you would do differently in future projects to avoid similar issues.

## Flash Light System
- After asking Copilot to help me create a Flashlight I noticed a bug, the code would work perfectly when I turned to face the left the code would not work as intended.
<video controls src="Broken Flashlight.mp4" title="Title"></video>
## Outcomes

### Source Code/Project Files
- Provide a link to your complete source code or project files.  
- Ensure the link is publicly accessible or shared with the appropriate permissions.  
- Include a brief description of the files provided, highlighting key components or any instructions required to run the project.

### Build Link
- Share a link to a playable or executable build of your project.  
- Ensure the build is accessible across relevant platforms and is publicly accessible.  
- Include any necessary instructions for running the build, such as system requirements or installation steps.

### Video Demonstration

# Camera System
https://github.com/user-attachments/assets/40c8aa02-0b36-4c1b-8484-994910464370
- First Attempt


- Embed a video or provide a link to a recorded demonstration of your project in action.  
- The video should showcase key features, functionality, and any unique elements of your project.  
- Include a brief commentary or text overlay in the video to explain the different aspects of your project as they are shown.

## Reflection
- After working in a group I relised that choosing reliable team members is a must, having just one team member not play their part can have a devastating effect on the production progress and put more work onto my plate in the longrun. After some thought my next game will be a solo project and I may use the original idea for my prototype.
### Research Effectiveness  
- Assess the usefulness of the research conducted during the project.  
- Highlight which sources (games, academic, documentation) had the most significant impact on your work and explain why.  
- Identify any research gaps or areas where additional information could have improved your project outcomes.

### Positive Analysis 
- I enjoyed working on this project applying what i know into the project to create a better and more efficient game then I would have been able to do before.

- I liked the challenge of creating a 2.5D game as it allowed me to learn how to do some things differently such as, changing the camera and movement systems.

- (Add Screenshots and other sources)

### Group Positive Analysis
- Working as a group has been positive in some ways as it is nice to give everyone their designated tasks to help split the workload as a whole.

- I enjoyed managing my group and giving them different asignments to help improve the game, from asking my artist to create different assets that will help improve the games overall storytelling, to asking my designer to create music using the different themes and instruments I chose to make the music more immersive and emotional.

- (add screenshots and other sources to help prove these statements)
- Reflect on the successful aspects of the project.  
- Highlight specific elements that worked well, such as technical solutions, creative decisions, or user feedback.  
- Provide evidence to support your analysis, such as test results, screenshots, or user comments.

### Negative Analysis  
- Identify the areas of the project that did not go as planned or could have been improved.  
- Discuss challenges you faced, whether technical, creative, or time-related, and evaluate their impact on the final product.  
- Reflect on any mistakes or missteps and what you learned from them.

### Next Time
- Outline what you would do differently if you were to undertake a similar project again.  
- Suggest improvements to your workflow, research methods, or implementation process based on your reflections.  
- Consider any new tools, techniques, or approaches you would explore in future projects to achieve better results.

## Bibliography  
- Compile a complete list of all sources referenced throughout your project. This may include articles, journals, videos, games, software, documentation, or any other materials.  
- Ensure all references are formatted according to the [university's citation method](https://mylibrary.uca.ac.uk/referencing).  
- Organise your references in alphabetical order. Alternatively, you may separate them by type (e.g., academic sources, games, videos), but consistency is key.

## Declared Assets
- Provide a detailed list of any third-party assets used in the project.  
- This includes asset packs, music, sound effects, 3D models, textures, scripts, or code from external sources.  
- Declare any use of AI tools (e.g., ChatGPT, GitHub Copilot, Meshy) or pre-existing code. Specify the purpose of these assets/tools and how they were integrated into your work.  
- Ensure you clearly distinguish between your original work and any external contributions to maintain academic integrity.
