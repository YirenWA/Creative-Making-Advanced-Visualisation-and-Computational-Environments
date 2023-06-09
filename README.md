# Creative Making-Advanced Visualisation and Computational Environments
## WEEK1
This week is primarily focused on establishing the background, theme, content, and form of the artwork.

### Inspiration  
The inspiration comes from daily life. Through observation, I have noticed that people leave many imprints in the physical world. Actions such as sitting, stepping, touching, and others leave visible traces in the physical environment. These traces roughly outline the contours and shapes of different parts of the human body. However, these forms also gradually disappear over time.  
In those intangible moments, can the imprints left by people condense within time?  

![trace](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/c80dc11d-3893-411c-942d-ddccc92b23a0)
From this discovery in life, divergent thinking was employed. Through group discussions, we decided to creat  a sensory game about the theme.  

### About Work  
It is an interactive game installation. This game represents an eternal memory world that extends human existence into a virtual and authentic digital space. There, the presence of individuals will be documented, and memories will solidify into digital imprints.  

Through the structure of physical spaces, participants will be guided to explore the digital world using physical actions in the real world and leave imprints in the digital space. In this digital world, there are no people or their shadows. Only the imprints of human remain.  
However, these imprints will gradually fade with time, so it is essential to leave lasting imprints within the limited intangible time.  

![sketch2-01](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/97249aec-e613-4fab-beac-45d81dff4981)

### Initial ideas for the Structure
Preliminary idea for Digital World Scene Construction: A conceptual visual composition with a sense of form, possibly using a frontal perspective. Visually, I want to present a memory world with a single color, providing participants with a ethereal and blurry visual experience.
The materials composing the digital space should assist participants in contemplating the gradual passage of time and its shaping influence on the world. It is important to highlight the flow of time and its impact on objects.    

#### Imprint options  
Choose a material to build the digital world in this project, which can be used for a series of game scenes in the future.   
Snow: It accumulates and melts with time. Its seemingly soft texture carries weight when subjected to external pressure. When instantly squeezed, it gives a sense of frozen time, leaving behind the harder parts.  
Sand: Time is like sand, taking shape when gathered and getting scattered by the wind as time passes.  
Moss: It grows slowly, requiring time to form. Therefore, moss can symbolize the continuity of time, the accumulation of processes, and the sedimentation of years.  
Vines, bubbles, and more.  

#### Physical space scene construction (sketch)  

![sketch](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/cf93bea0-e938-4b49-b10b-13644af1e356)  
Consider the playability of the space for people and its correspondence to the structure of the digital space. Overall, it should resemble a "child" playground.  


## WEEK2
This week was mainly focused on determining the technical equipment to be used through group discussions. And I also started with the initial design of the two spaces.   

#### Using Blender for modeling  
I created a digital world with a certain level of surrealism, capturing a sense of erosion over time. The composition includes elements such as buildings, screens, stairs, gates, curtains, and chairs, all closely related to human life. Everything in the scene can be floating, distorted, and seemingly unrelated objects, yet they are interconnected, forming a loop. This world resembles an unbalanced yet egalitarian amusement park for humans.  

![1](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/9ab3f174-15e7-484a-8d7a-ad260e60d35e)

In the group discussion, the team member provided technical solutions to my proposed idea, and we ultimately decided to train a neural network to utilize cameras for recognizing human interactions within Unreal Engine.  

#### In the construction of the physical scene  
I have carried forward the preliminary ideas from the first week. Considering feasibility, I combined the first and second plans in the design. Corresponding to the front-to-back and up-and-down relationships modeled in the digital world, I designed a rough framework.

I measured the different heights at which people sit, stand, and reach, and ultimately built a space measuring 1.35 * 1.8 * 1.8m. The vertical space is divided into three levels. Through group discussions, we concluded that the occlusion relationship from front to back also affects recognition, so the spatial relationship from front to back is progressive.  

![structure](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/744fef88-2d98-4f94-a036-de2fdc246bd3)
 

## WEEK3
本周主要是搭建了物理空间，并将数字空间在unreal 进行了视觉上的美化。  
购买计算切割材料  
由于物理空间的复杂性和可玩性，所以要确保框架具有稳定结构，并在前后与上下空间的对应进行了测试
![process-01](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/028f0b38-cee0-4e04-88d5-63d23ca4274e)

物理场景搭建  
unreal 特效（粒子做雪，物体mesh粒子，贴图texture绘图设计，地面/画面场景的设计）  
问题：建模mesh的粒子特效，分布不均匀。 
![Niagara mesh？不均匀](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/8cc0b26e-cca7-4f08-bdf3-4d5d3321b207)

视觉效果调整美化

## WEEK4
调试  
拍摄  
视频剪辑

## Future
多个材质场景
识别不止头顶
有各种姿势，具体的印记。
