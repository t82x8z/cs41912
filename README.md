java cAssignments Creative 2 Grading  Examples
Grading  Examples
If you want a safe and straightforward path to a full completion grade, we suggest picking two
technical features mentioned on this page and implementing them. If your group implements two
technical features reasonably well, even in a scene with pretty boring composition, we will at least
give you completion credit. Some technical features could be worth more than others, and the
value may be greater for especially impressive execution of a technical feature. But implementing
two features reasonably well is what we will consider ``full completion".
You can also use the obj loader included in the code to load simple models. The most
straightforward way to create such models would be to use Blender. Blender is free and open
source, and there are lots of tutorials online that show how to use it. With an un-accelerated ray
tracer written in Python you won't be able to render very complex models, but you can certainly
still do a lot with low polygon content.
USING TOOLS LIKE BLENDER
See Exporting from Blender for tips on how to use Blender, an open source cross-platform
3D modeling tool, to help you create and export models. If you use 3D asset files in your
scene, be sure to identify what parts of the scene were loaded from files, and how you
obtained or created those files! As you will see in several of the examples below, you can do
a lot of cool stuff without the aid of 3D modeling software, but tools like Blender are an
option for you.
Scene Composition:
Good composition matters, and in extreme cases may even compensate if your technical features
are a bit lacking. The philosophy here is that making particularly good use of the basics can
demonstrate strong understanding of the fundamentals, which deserves its own reward.
COMPOSITION AS A SELLING POINT
If you plan to focus on creating a compelling composition, anticipate spending time on trial
and error. A lot of care went into placing spheres, camera, and lights in these scenes. Try to
set up an efficient pipeline for exploring these options early on, so you can quickly iterate
and find parameters that look best.
For example, the example below from a few years ago makes particularly good use of spheres and
lighting to create a compelling composition. Note that this submission might be less than full
completion were it submitted this year, as the time and requirements for the project have
increased, but it was strong for its year and remains a good example of how basic elements can
be combined to create a compelling scene.
Kirby in Space, by Yingshi Zhu and Mandy Kwok
Potential Technical Features
A reasonably composed scene with at least two well-executed technical features is probably the
safest way to ensure full completion credit on this project.
STRATEGIC FEATURE COMBINATIONS
Think about what features to prioritize and how certain feature might complement each
other. For example, some features might substantially increase computation time, which
could be offset by choosing to implement an acceleration structure for ray intersection (e.g.,
a k-d tree) as another one of your features.
BE ACCURATE IN YOUR REPORTS!
Your technical feature needs to work (at least excluding very edge cases). Do not claim that
you have implemented something that you have not; we will check suspicious claims, and
you will be penalized if they are inflated. In particularly egregious (e.g., deliberate-looking)
cases, false claims may be treated as academic dishonesty.
Some ideas to consider include:
Extended Obj Loader  Custom Meshes: The current obj loader provided in A4 will only
work with simple obj files that have 1 mesh. However, it should not be hard to extend it into an
obj loader that can handle multiple meshes. The read_obj and read_obj_triangles
functions in A4 , along with cube.py scene example should be helpful for you to learn from,
and experiment with. You can also create some obj files with multiple meshes in Blender,
and analize those files to implement your own loader. With such Extended Obj Loader , you
can export custom composition elements t代 写program、Python
代做程序编程语言hat you create in Blender. One strategy is to even
use Blender to compose your full scene, including hte camera position and parameters, in
Blender and export it for rendering in your ray tracer.
Additional geometric primitives: you can add new primitives, implement their ray
intersection calls, and use them to create new shapes. Note that a primitive that is simply an
array of existing primitives does not count as a new primitive (e.g., the cube is just a
collection of simple triangles). One simple shape may not be treated as a complete extra
feature, either (e.g., a plane). Shapes like a torus or cone are good choices.
Constructive solid geometry (CSG): implement boolean operations on existing primitives.
E.g., the intersection of two spheres can create a pretty cool flying saucer shape....
Additional shading modes or phenomena: E.g., refraction, or more general BRDFs, E.g.,
Fresnel reflection
Refraction, caustics, lensing
Scattering
Surface Texture Mapping: Various types of texture mapping including
Diffuse texture mapping
Displacement mapping
Normal Mapping
Bump Mapping
Ray-intersection Acceleration structures: You could implement code to make ray tracing
faster. We haven't discussed this much in class, but I have addad a bonus video from Steve
on the topic to Canvas, and if you are interested it is certainly google-able as well. Make sure
you describe this type of feature clearly in your submission, as it won't necessarily be visible
in your image. Also, this feature works best if you use it to ray trace a higher resolution, more
anti-aliased, and/or more complex scene with more complicated effects. Report speed gains
you get on at least one test scene with your machine in your report. Also note that we can
and do check to see that you actually implemented what you say you did here...
UFO Scenes
These images show a UFO created where the saucer was created using constructive solid
geometry. The saucer of the UFO is the intersection of two spheres. The top and bottom of the
ufo have additional spheres as well.
In our first UFO scene we render the UFO above some paraboloid grass hills:
Composition for this image is a bit weak. It technically has two features (CSG and paraboloid
intersection), but both are only very basic implementations. It would probably end up getting
close to full completion credit, but not more.
In our second UFO scene we render the UFO above the desert ground (UFOs like the desert).
Here, the desert is rendered with a normal map and a diffuse texture map.
This image also has two features (CSG and normal mapping). The technical features are pretty
similar to the image above, but the composition is much stronger. It uses several lights to create
dramatic lighting on the ground and make it look like the bottom of the UFO is glowing. This image
would probably get full completion credit, maybe even a bit extra depending on how your TA's feel
it compares with other submissions.
Submissions from Previous Years
Alan Liu and Selina Xiao (2023)
These two implemented ellipsoid cylinder and cone primitives, constructive solid geometry,
texture mapping, and a cool composition.
Ethan Yang and Peter Wu (2023)
These two implemented a path tracer, refraction, thin lens approximation with defocus, texture,
displacement, and normal mapping... This was a really ambitious submission, and many have
failed to implement much less ambitious lists of features.
CSG and Ellipsoids by Ruyu Yan and Becky Hu
This submission has nicely implemented CSG, as well as ellipsoids, some new material, and great
composition.
Solar Donut Dolly Zoom by Dubem Ogwulumba
and William Ma
The top submission from 2021
Some 2022 Examples
Prithwish Dan  Simon Kapen
Very impressive use of constructive solid geometry. The entire scene is made from CSG by
combining various basic shapes.
Sissel Sun  Claire Zhou
Nicholas Broussard  Orion Tian
Jack Otto and Sean Brynjolfsson
This one was rendered using fractals, which lend themselves well to accelerated ray tracing of
very complex geometry.
Edit this page

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
