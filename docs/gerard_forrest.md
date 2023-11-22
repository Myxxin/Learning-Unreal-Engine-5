# Ultimate Forest Course


https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/8a65bc4d-a17a-455b-853e-ea13d4b71cc9


https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/6af97ad8-4d5a-4b05-93b1-701025d2cc6f



I enjoyed the course, but it was also a lot of work. 

In the first third I learned the basics of Speedtree, which is a procedural software specific for the creation of vegetation assets.

![image](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/9c5a4341-e530-4d82-939f-d1aaba11b141)


Thanks to my slight experience with Houdini, it was easy to get into and I learned how to optimise foliage for real-time contexts along the way. Since I didn’t have any experience with 3d modelling before the course, I picked up a lot of 3d basics too. For the textures, I used Quixel‘s photogrammetry library. 
While I followed the tree tutorials pretty closely, I deviated quite a bit for the ground foliage. My overall favourite creation is this fern:

![SM_Fern_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/9406a0e5-f907-4075-bf82-79ffbc370644)

To save performance, I only used Nanite for the tree stumps, the tree leaves and ground foliage rely on LODs.

To prepare the final scene in Unreal, I had to create a lot of shaders for the landscape, the Megascan assets and of course the vegetation.
While the first functions to control the color, roughness etc. were manageable, the shaders became a bit too complicated too quickly. Especially the Auto-Landscape Material with its different layers, vertex painting and (in UE5.1 extra tricky)tesselation was a challenge. The instructor unfortunately failed to explain the mathematical concepts behind most of the functions. The quality of all the final shaders is however a definite improvement over their default counterparts.

![image](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/02828e2c-4f77-44e1-a18a-cd22ab3d8421)

With this as a solid technical fundament, I created the landscape in worldcreator on my own. The instructor used the in-engine tools for this this task, but I wanted to try out something more procedural and better simulated. I really enjoyed this piece of software! It uses the GPU for all calculations and is therefore able to run in real-time, which allows for great artistic control. I have barely scratched its surface.

![TW3_Forrest_Path_1](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/58ad0f23-8303-4dd4-b655-3539a3b52c10)


I also created some background assets which I didn’t use in the end.

![DistantMountain_TW3_0](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/87d01653-a83d-4770-8225-1432647a5f86)
![image_2023-08-01_18-55-13](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/236754fc-9efe-49b8-b8ec-4bf42f55aa4f)



After importing the landscape, I started to populate it by using the procedural foliage tools, which spawned my assets within a volume. While the end result looks fairly natural, it was a clunky experience to get there and I will definitely use the PCG system in the future. 

Oh, and I also made some ground textures in Quixel Mixer:

![Rock](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/51ced8cb-704f-417f-9331-754b7f8af622)
![ForrestFloor](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/6eec44ca-11a1-432c-ac5e-475cb1a95464)


The particles and insects are some very simple nanite systems and for the local animated volumetric fog, I used these blueprints in addition to this fog algorithm.

For the lighting, I preferred to use virtual shadowmaps over raytraced shadows. They unrealistically sharp, but created a nice look in combination with the many tree branches. 
I rendered the final shot with DLA and movie render queue and... that's it!! :)



https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/87681b6c-f309-49d5-b74a-852968b89a12



I will probably return to the this project to redo the lighting at some point to achieve a more realistic result compared to the game-y look above. 
In total, I spent about 95 hours with this course. 

Here are some lowquality render of all my assets and some extras :)
![SM_Grass_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/43748740-01ec-4f9a-a18e-924ca645eea8)
![SM_Daisy_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/c32ed41f-b993-465b-a645-13a3709e6915)
![SM_Crownbeard_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/13a5f431-7a93-4e39-a07b-6d4de676fad7)
![SM_Aspen_Stump_1b](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/8bbbcf1e-492d-41f2-a924-1d61304991d7)
![SM_Aspen_Sapling_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/253d7959-283b-4ce1-810d-d3bdcf1417bd)
![SM_Aspen_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/19dc9ade-8e94-4ae4-b159-fdd77e1d2004)
![SM_Pine_Sapling_1a_detail](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/778ba5e4-2430-4ab9-a08e-af5c5261d33d)
![SM_Pine_Sapling_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/c00cac77-32f5-406b-8299-f0eced50e79b)
![SM_Pine_1a_detail](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/dd5e3ef5-45b2-431e-bd08-4eeabb6c024f)
![SM_Pine_1a_Branch](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/f81755e6-92c7-4bbf-bc4a-7d24283cbecf)
![SM_Pine_1a](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/df1fcd81-4ea7-4f64-b467-747181a2fcf6)


![HighresScreenshot00016 - Kopie](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/0122dc1b-e1b6-4bd5-9fda-3d4f3cd13a1f)

![image_2023-07-16_20-30-59](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/19ba736c-1b5b-4be4-bf54-49d453fd9b01)

![image_2023-08-04_17-49-11](https://github.com/Myxxin/Learning-Unreal-Engine-5/assets/93442123/daa18a5d-c878-4d6f-969a-00a639a7212a)

