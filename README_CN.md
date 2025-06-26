# 基于机械臂的肖像绘制系统

[English](README.md) | 简体中文 |

**_2023.4~2023.6_**

_三人团队项目_

<div align=center>
<img src="https://github.com/anOrangeCat3/anOrangeCat3/blob/main/gif/6_1750689850-ezgif.com-video-to-gif-converter.gif"/>
</div>


**_项目描述:_** 本项目是一个机器人控制课程的课设，主要内容是使用机械臂绘制肖像素描。流程从输入一张真实的肖像照片开始，接着通过图像处理技术提取出肖像的轮廓，并将其转换为一系列有序的坐标点。这些坐标点作为机械臂运动的路径。最后，控制机械臂沿着生成的路径运动，从而完成肖像的绘制。

**_个人贡献:_** 我通过排序后的像素坐标生成了机械臂的路径，并掌握了使用机械臂厂商提供的 **ROS** 控制包进行基础控制。我还使用了 **PID 控制算法** 来控制机械臂，以实现绘图功能。

本项目主要使用 Python 编程语言，并借助机械臂厂商提供的 ROS 控制包进行基本操作。

**_项目视频链接:_**

_youtube:_ https://www.youtube.com/shorts/PwJzDzVUQ28

_bilibili:_ https://www.bilibili.com/video/BV1Uw411k7TE

我的两位队友负责 **图像处理部分**，包括从输入的肖像图像中提取轮廓和点、对点进行排序和分组，以表示不同的笔画。

我主要负责 **机械臂控制部分**，确保机械臂按照排序后的坐标点运动，从而完成整幅作品。

**_以下是相关文件:_**

|文件夹名/文件名|内容与功能|
|------|-----|
|_StickFigure_|**初步图像处理，提取人物轮廓。**|
|_final_project_|**整合所有程序，形成完整的工作流程：输入照片，自动提取轮廓、取点、规划路径并控制机械臂完成绘画。**|
|_img2points_|**提取轮廓、选点、排序、确定笔画，最终生成机械臂路径。**|
|_Final report.pdf_|**项目最终报告，详细介绍了所有技术细节。**|
|_Pre_final.pptx_|**最终项目展示的 PPT**|
|_Project proposal.pdf_|**项目立项书，主要介绍参考文献以及市面上已有的绘图/书写机器人。**|
|_opening_pre.pptx_|**项目开题展示 PPT**|

**_图像处理的部分结果如下所示:_**

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/3c7d9f0e-0fa6-42d3-af2c-7b6bc0e16ac8"  />
</div>

控制部分主要采用了 **PID 控制**，但由于硬件精度限制，机械臂各个关节主要使用 **PD 控制**。部分参数如下图所示：

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/9da2936b-0ed6-4b61-b709-8116c665cbd1"  />
</div>

**_最终绘图结果如下图所示:_**

<div align=center>
<img src="https://github.com/anOrangeCat1/projects_sustech/assets/99580008/0e1ae695-f4aa-4b16-98c6-d66303c3f6a0"  />
</div>
