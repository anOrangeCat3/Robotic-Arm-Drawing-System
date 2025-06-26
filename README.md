# A Robotic Arm-Based Portrait Drawing System

English | [简体中文](README_CN.md) | 

**_2023.4~2023.6_**

_Team Project of 3 members_

<div align=center>
<img src="https://github.com/anOrangeCat3/anOrangeCat3/blob/main/gif/6_1750689850-ezgif.com-video-to-gif-converter.gif"/>
</div>

**_Discription of project:_** This is a project for a robot control course. It involves using a robotic arm to draw portrait sketches. The process begins with inputting a real portrait photograph. Image processing techniques are then applied to extract the outline of the portrait, which is transformed into a series of ordered coordinate points. These points serve as the path for the robotic arm to follow. Finally, the robotic arm is controlled to move along the generated path, ultimately completing the portrait drawing.

**_Individual contribution:_** I formed a path for the robotic arm by using the sorted pixel coordinates and became proficient in utilizing the **ROS** package provided by the robotic arm manufacturer for basic control. I applied the **PID control algorithm** to control the robotic arm for the purpose of creating artwork. 


This project primarily utilized Python programming. It also used the ROS package provided by the robotic arm manufacturer for basic control. 

**_video link:_**

_youtube:_ https://www.youtube.com/shorts/PwJzDzVUQ28

_bilibili:_ https://www.bilibili.com/video/BV1Uw411k7TE

My two teammates were responsible for **image processing part**, which involved extracting the contours and points from the input portrait images, sorting and grouping the points to represent different brush strokes. 

I was primarily responsible for **robotic arm control part**, ensuring that the robotic arm moved according to the sorted coordinate points to complete the artwork.


**_Below are the relevant files:_**

|folder_name/file_name|content&function|
|------|-----|
|_StickFigure_|**Preliminary image processing, extracting the outline of the human subjects.**|
|_final_project_|**Integrate all programs to form a complete workflow: input a portrait photo, automatically extract the outline, take points, plan the route, and control the robotic arm to complete the painting.**|
|_img2points_|**Extract the outline, select points, sort them, determine the brushstrokes, and finalize the robotic arm's path.**|
|_Final report.pdf_|**Final Report, providing detailed information about all the technical aspects of this project.**|
|_Pre_final.pptx_|**The final project presentation PPT**|
|_Project proposal.pdf_|**Research Proposal, mainly introducing the referenced articles and the current drawing or writing robots on the market.**|
|_opening_pre.pptx_|**The opening presentation PPT**|

**_The image processing results are shown as below:_**

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/3c7d9f0e-0fa6-42d3-af2c-7b6bc0e16ac8"  />
</div>

For control part, primarily, we used **PID control**. However, due to limitations in hardware precision, the joints of the robotic arm mainly employed **PD control**. Some of the parameters are shown in the figure below：

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/9da2936b-0ed6-4b61-b709-8116c665cbd1"  />
</div>

**_The final result is depicted in the following image:_**

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/0e1ae695-f4aa-4b16-98c6-d66303c3f6a0"  />
</div>




