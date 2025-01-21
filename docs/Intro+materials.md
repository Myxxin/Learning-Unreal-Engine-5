# Introduction Course
[Unreal Sensei - Unreal Engine 5 Beginner Tutorial](https://www.youtube.com/watch?v=k-zMkzmduqI)

This course provided a good introduction to the Unreal Engine UI and UX, to Lighting, Materials, Blueprints and Environment art.

![alt](/docs/imgs/castle1.png)
![alt](/docs/imgs/castle2.png)
![alt](/docs/imgs/castle.png)


I decided to abandon the environment and to skip the final details and the rendering. Though I managed to give the scenen a little bit of an identity with the sky and the lighting, it wasn't really my cup of tea, especially in terms of workflow. I however still learned a lot, especially regarding my plans going forward:

* I enjoy working with foliage and want to learn how to create realistic biomes
* I really enjoy lighting scenes with lumen
* I enjoy the Unreal engine UI
* I don't enjoy working with Kitbash assets such as the castle, I'd rather create finished assets in Blender.

Overall, I spent 15h on this introduction of which about 10h where spent on the final environment due to the very manual workflow.

# Material Course

To extend my knowledge of the Material Graph, I took a [course on the subject by Vince Petrelli](https://www.udemy.com/course/unreal-engin5-one-course-solution-for-material/?couponCode=BFCPSALE24).

I started off the course by creating some simple effects materials, my favourite ones being this basic fire material and dissolve effect.

![fire](/docs/imgs/fire.png)

![dissolve](/docs/imgs/dissolve.png)

## Master Material

In the next part I created a very typical Master-Material. 
While I already knew most of the techniques introduced here, it was still useful to get a back-to-basics introduction to the PBR workflow and its components. The covered topics were:

### UV
![alt text](/docs/imgs/image-1.png)

## Albedo
![alt text](/docs/imgs/image-2.png)

## Metallic
![alt text](/docs/imgs/image-3.png)

## Specular
![alt text](/docs/imgs/image-4.png)

## Roughness
![alt text](/docs/imgs/image-5.png)

## Normals
![alt text](/docs/imgs/image-6.png)

## Ambient Occlusion
![alt text](/docs/imgs/image-7.png)

I also decided to implement Nanite Displacement:
![alt text](/docs/imgs/image-8.png)

## Layering

The next chapter covered how to layer and blend materials and decals to create convincing realistic scenes with a lot of variation:
![alt text](/docs/imgs/image-9.png)
![alt text](/docs/imgs/image-10.png)
![alt text](/docs/imgs/image-11.png)

## Landscape Material
The final chapter covered the creation of a landscape material. 
To my surprise, this was the least interesting course for me, as I knew all the techniques presented here already and once again realised that landscape materials are, in my opinion, overrated.

I will not show the entire material here as it is quite complicated, here is just all the parameters for the Slope Mask Material Function:

![alt text](/docs/imgs/image-12.png)

In summary, my main issue is that even with a very detailed landscape material such as this, the quality of the landscape is still extremely low compared to using dedicated assets.

![alt text](/docs/imgs/image-13.png)

# Substrate Exploration

After the end of the course, I explored the (relatively) new Substrate toolset, which allows for physically more accurate materials with intricate lighting details.
Here, I used it to create strange alien textures:

![alt text](/docs/imgs/image-14.png)
![alt text](/docs/imgs/image-15.png)
![alt text](/docs/imgs/image-16.png)
![alt text](/docs/imgs/image-17.png)
![alt text](/docs/imgs/image-18.png)

Finally, I started working on this scene, but in the end did not finish it:
![alt text](/docs/imgs/image-19.png)
