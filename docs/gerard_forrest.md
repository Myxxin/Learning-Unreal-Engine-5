# Ultimate Forest Course

I enjoyed the course, but it was also a lot of work. 

In the first third I learned the basics of Speedtree, which is a procedural software specific for the creation of vegetation assets.

Thanks to my slight experience with Houdini, it was easy to get into and I learned how to optimise foliage for real-time contexts along the way. Since I didn’t have any experience with 3d modelling before the course, I picked up a lot of 3d basics too. For the textures, I used Quixel‘s photogrammetry library. 
While I followed the tree tutorials pretty closely, I deviated quite a bit for the ground foliage. My overall favourite creation is this fern:

To save performance, I only used Nanite for the tree stumps, the tree leaves and ground foliage rely on LODs.

To prepare the final scene in Unreal, I had to create a lot of shaders for the landscape, the Megascan assets and of course the vegetation.

While the first functions to control the color, roughness etc. were manageable, the shaders became a bit too complicated too quickly. Especially the Auto-Landscape Material with its different layers, vertex painting and (in UE5.1 extra tricky)tesselation was a challenge. The instructor unfortunately failed to explain the mathematical concepts behind most of the functions. The quality of all the final shaders is however a definite improvement over their default counterparts.

With this as a solid technical fundament, I created the landscape in worldcreator on my own. The instructor used the in-engine tools for this this task, but I wanted to try out something more procedural and better simulated. I really enjoyed this piece of software! It uses the GPU for all calculations and is therefore able to run in real-time, which allows for great artistic control. I have barely scratched its surface.

I also created some background assets which I didn’t use in the end.

After importing the landscape, I started to populate it by using the procedural foliage tools, which spawned my assets within a volume. While the end result looks fairly natural, it was a clunky experience to get there and I will definitely use the PCG system in the future. 

The particles and insects are some very simple nanite systems and for the local animated volumetric fog, I used these blueprints in addition to this fog algorithm.

For the lighting, I preferred to use virtual shadowmaps over raytraced shadows. They unrealistically sharp, but created a nice look in combination with the many tree branches. 
I rendered the final shot with DLA and movie render queue and... that's it!! :)

I will probably return to the this project to redo the lighting at some point to achieve a more realistic result compared to the game-y look above. 