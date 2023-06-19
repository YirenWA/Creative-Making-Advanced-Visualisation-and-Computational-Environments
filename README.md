# Creative Making-Advanced Visualisation and Computational Environments  
"CHRONOSCAPE" Video Link: https://www.youtube.com/watch?v=oIYKefJnTX8
## WEEK1
This week is primarily focused on establishing the background, theme, content, and form of the artwork.

### Inspiration  
The inspiration comes from daily life. Through observation, I have noticed that people leave many imprints in the physical world. Actions such as sitting, stepping, touching, and others leave visible traces in the physical environment. These traces roughly outline the contours and shapes of different parts of the human body. However, these forms also gradually disappear over time.  
In those intangible moments, can the imprints left by people condense within time?  

![trace](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/c80dc11d-3893-411c-942d-ddccc92b23a0)
From this discovery in life, divergent thinking was employed. Through group discussions, we decided to creat a MR Experience Game about the theme.  

### About Work  
It is an MR game. We created an everlasting memorial worldthat extends human existence into a virtual and authentic digital space—a frozen testament to existence and the passage of time. There, the presence of individuals will be documented, and memories will solidify into digital imprints.  

Through the structure of physical spaces, _participants will be guided to explore the digital world using physical actions in the real world and leave imprints in the digital space._ In this digital world, there are no people. Only the imprints of human remain. However, these imprints will gradually fade with time, so it is essential to leave lasting imprints within the limited intangible time.  

![sketch2-01](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/97249aec-e613-4fab-beac-45d81dff4981)

### Initial ideas for the Structure
Preliminary idea for Digital World Scene Construction: A conceptual visual composition with a sense of form, possibly using a frontal perspective. Visually, I want to present a memory world with a single color, providing participants with a ethereal and blurry visual experience.
The materials composing the digital space should assist participants in contemplating the gradual passage of time and its shaping influence on the world. It is important to highlight the flow of time and its impact on objects.    

#### Imprint options  
Choose a material to build the digital world in this project, which can be used for a series of game scenes in the future.   
__Snow:__ It accumulates and melts with time. Its seemingly soft texture carries weight when subjected to external pressure. When instantly squeezed, it gives a sense of frozen time, leaving behind the harder parts.  
__Sand:__ Time is like sand, taking shape when gathered and getting scattered by the wind as time passes.  
__Moss:__ It grows slowly, requiring time to form. Therefore, moss can symbolize the continuity of time, the accumulation of processes, and the sedimentation of years.  
Vines, bubbles, and more.  

#### Physical space scene construction (sketch)  

![sketch](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/cf93bea0-e938-4b49-b10b-13644af1e356)  
Consider the playability of the space for people and its correspondence to the structure of the digital space. Overall, it should resemble a "child" playground.  


## WEEK2
This week was mainly focused on determining the technical equipment to be used through group discussions. And I also started with the initial design of the two spaces.   

### Define the game structure  

In the group discussion, the team member provided technical solutions to my proposed idea, and we ultimately decided to train a neural network to utilize cameras for recognizing human interactions within Unreal Engine.  
Our objective is to design an immersive playground that magnifies and commemorates the impact individuals have made. We have constructed a physical setting that mirrors a virtual world in terms of its structure and form. By deploying neural networks, we are able to track the positions of people in the real world and project their movements onto the virtual realm. This experimental mixed-reality game blends the realms of neural networks and reality. The aim for our players is to leave behind a multitude of captivating and significant traces within this interconnected world.   

#### Using Blender for modeling  
I created a digital world with a certain level of surrealism, capturing a sense of erosion over time. The composition includes elements such as buildings, screens, stairs, gates, curtains, and chairs, all closely related to human life. Everything in the scene can be floating, distorted, and seemingly unrelated objects, yet they are interconnected, forming a loop. This world resembles an unbalanced yet egalitarian amusement park for humans.  

![1](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/9ab3f174-15e7-484a-8d7a-ad260e60d35e)

#### In the construction of the physical scene  
I have carried forward the preliminary ideas from the first week. Considering feasibility, I combined the first and second plans in the design. Corresponding to the front-to-back and up-and-down relationships modeled in the digital world, I designed a rough framework.

I measured the different heights at which people sit, stand, and reach, and ultimately built a space measuring 1.35 * 1.8 * 1.8m. The vertical space is divided into three levels. Through group discussions, we concluded that the occlusion relationship from front to back also affects recognition, so the spatial relationship from front to back is progressive.  

![structure](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/744fef88-2d98-4f94-a036-de2fdc246bd3)
 

## WEEK3
This week, my main task was to set up the physical space and create Niagara effects, visual adjustments, and other work for the digital world in Unreal Engine.  

#### Physics Scene Construction  
I calculated and purchased wood for cutting. Due to the complexity and playability of the physical space, I wanted to ensure that the framework had a stable structure, so I conducted tests on the relationships between the front and back, as well as the upper and lower spaces.   

![process-01](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/028f0b38-cee0-4e04-88d5-63d23ca4274e)
  
#### Unreal effects creation    
I made the particle effect of object collision static mesh Disintegration to make the traces of people touching space.   
We use a displacement shader graph to overlap the original material, thus create a transparent displacement effect. We placed a ball in the center to indicate the position, but we made it transparent. We also use the displacement map as the particle map, thus particles can emit from the edges of the displaced area and also light up the entire scene.  

![碰撞粒子](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/530e2290-301e-4787-bbd9-a1ba3f84a392)

![碰撞粒子1](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/36e240e1-9678-4b84-a85d-4b0e0d40600e)


I made the main model its mesh particles to enrich the visual effect.  
Problem: Initially, the model's mesh particles were unevenly distributed, which I solved by checking the box to support (GPU) uniformly distributed sampling. 

![Niagara mesh？不均匀](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/8cc0b26e-cca7-4f08-bdf3-4d5d3321b207)

I created some weather effects with Niagara particles to create a visual impression.  

![B2](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/45b7bae1-b2c0-4b26-a982-18c4554a8c16)

Mapping texture design. I also painted the texture design for the traces. (Not used in the end)  

![贴图](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/e5f87b96-5194-46f1-a922-9443f3375040)

#### Neural Network (Work of team members)  
For our project, the detection of people from top view is crucial as the camera is the only input that analyze the real-world scene and the position data for further interactions. As we have gained experience on deployment of neural network in game engine via previous projects, we chose to deploy a convolutional neural network as the detection algorithm. To load a neural network in Unreal Engine, we decided to use OpenCV library which can load various types of neural network via its DNN module.   

_Because it is a top recognition, it can only affect the relationship between front and back, the relationship between top and bottom cannot be done, so it is necessary to change the height at which the interacting objects can reach. However, in future designs, multiple recognition can be used and specific traces can be left._

## WEEK4  
This week is mainly about debugging and testing, and finally scene building and filming.  

![调整测试](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/0cd88e64-87cd-4e6a-82bc-2089da0fe594)  

![搭建](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/b14df617-1941-4064-9cdf-4aff0ef537ff)  

![测试_04008](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/6af94965-d812-4097-8292-08ee03b25868)

## Game showcase

![效果_01438](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/c9a3437b-f9b7-4b2b-939b-9898c3ee31a7)  

![测试1_01874](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/67530650-3f46-4924-a368-a0a793f8b9ed)

![效果_00399](https://github.com/YirenWA/Creative-Making-Advanced-Visualisation-and-Computational-Environments/assets/119879041/01aeb312-4c27-4d6c-84da-cb750c63994a)

