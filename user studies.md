# user studies

### questionnaire

#### The score for the quality of mesh generation ####

It can be considered from the following aspects: the quality of geometric details in the generated 3D meshes, the topological quality of the 3D meshes, the performance of the generated 3D grids in meeting task requirements, and the consistency and reliability of the generated results.

```
How would you rate the quality of the generated 3D meshes in terms of geometric details (e.g., smoothness, precision)?         
(1 = Very poor, does not meet requirements; 9 = Excellent, fully meets requirements)
```

```
How satisfied are you with the topology quality of the generated 3D meshes (e.g., no broken areas, no redundant faces)?
(1 = Very dissatisfied; 9 = Very satisfied)
```

```
How well do the generated 3D meshes meet the requirements of your specific tasks (e.g., rendering, simulation, or 3D printing)?
(1 = Completely unsuitable; 9 = Completely suitable)
```

```
How consistent and reliable are the generated results (e.g., stable quality across different generations)?
(1 = Very inconsistent; 9 = Very consistent)
```

#### The score for how helpful to work ####

The following aspects can be considered: whether the generated 3D meshes enhance modeling efficiency, to what extent the method of generating 3D models aids in reducing manual modeling, and whether the generated meshes lower the skill threshold required for the task.

```
How much has the generated 3D mesh helped improve your modeling efficiency?
(1 = No improvement; 9 = Greatly improved efficiency)
```

```
Compared to traditional 3D modeling methods, how much has this generation method reduced the need for manual adjustments or fixes?
(1 = No reduction; 9 = Significant reduction)
```

```
Has the generated mesh lowered the skill barrier for tasks, making complex modeling more accessible to non-experts? If so, to what extent?
(1 = No skill barrier reduction; 9 = Significant reduction)
```

### User Feedback

**Scores for each question**

| user &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | &nbsp; &nbsp; &nbsp;  1.1   &nbsp; &nbsp; &nbsp;       | &nbsp; &nbsp; &nbsp;  1.2     &nbsp; &nbsp; &nbsp;    | &nbsp; &nbsp; &nbsp;  1.3     &nbsp; &nbsp; &nbsp;   |  &nbsp; &nbsp; &nbsp; 1.4    &nbsp; &nbsp; &nbsp;    | &nbsp; &nbsp; &nbsp;  2.1    &nbsp; &nbsp; &nbsp;      |  &nbsp; &nbsp; &nbsp; 2.2   &nbsp; &nbsp; &nbsp;     | &nbsp; &nbsp; &nbsp;  2.3  &nbsp; &nbsp; &nbsp;       |           
| :---     |    :----:   |   :----:   |    :----:  |   :----:    |    :----:   |   :----:    |    :----:   |  
| U1       | 9 | 9 | 8 | 8 | 6 | 7 | 9 |
| U2       | 6 | 8 | 9 | 9 | 6 | 8 | 8 |
| U3       | 7 | 8 | 8 | 7 | 7 | 9 | 8 |
| U4       | 9 | 8 | 9 | 6 | 9 | 9 | 7 |
| U5       | 8 | 6 | 8 | 6 | 6 | 9 | 7 |
| U6       | 6 | 4 | 5 | 9 | 7 | 4 | 7 |
| U7       | 8 | 5 | 6 | 5 | 4 | 7 | 5 |
| U8       | 8 | 6 | 4 | 9 | 7 | 6 | 8 |
| U9       | 9 | 7 | 9 | 5 | 6 | 5 | 9 |
| U10      | 8 | 6 | 8 | 4 | 9 | 4 | 6 |
| U11      | 8 | 4 | 7 | 6 | 5 | 6 | 5 |
| U12      | 6 | 9 | 6 | 9 | 4 | 8 | 8 |
| U13      | 8 | 9 | 9 | 4 | 9 | 4 | 7 |
| U14      | 5 | 5 | 5 | 7 | 4 | 5 | 6 |
| U15      | 7 | 4 | 7 | 6 | 5 | 7 | 8 |

#### Background ####
We have selected 3 representative professionals from the 15 users in the 3D industry to answer the following questions: 

**U1**: Simulation Character Design Engineer, primarily responsible for simulating and character emotion modeling, requiring models with high-resolution details, animation-ready topology, and materials compatible with PBR workflows; 

**U6**: Scene Virtual Reality Engineer, primarily in charge of segmenting scenes and creating 3D scenes designs for virtual reality projects or architectural visualizations. They require complex scenes, realistic materials, and efficient generation workflows.

**U15**: Video Generation and Special Effects Engineer, who specializes in the video industry, focuses on creating 3D models for visual effects, which often need to integrate with simulations and dynamic environments. They require highly detailed and dynamic meshes compatible with special effects workflows.

#### Questions about subsequent improvements ####

1. What aspects of the generated 3D meshes do you think need improvement? For example: higher resolution, fewer topology issues, or more realistic textures.

      **U1**: We need extremely detailed models, such as facial expressions, muscle textures, and skin pores. The generated meshes should support high-resolution details while maintaining clean topology for further refinement in sculpting tools like ZBrush. Optimized topology. To ensure compatibility with animations, we requires clean topology, especially in deformable areas like joints and facial regions. Current generated meshes might exhibit irregular topology, such as excessive triangles or broken edge flows. Improvements should focus on quad-dominant topology suitable for rigging and animation. Optimized UV layouts. Generated meshes often have overlapping or inefficient UV layouts. We expects pre-optimized UVs with proportional space allocation for different areas (e.g., higher resolution for the face, lower resolution for the body).

      **U6**: Current tools may focus on generating single objects, but interior designers need support for generating entire scenes, such as complete room layouts with walls, ceilings, floors, and furnishings automatically placed. Since interior scenes often include many complex objects, we need meshes optimized for lower polygon counts while maintaining visual quality, enabling smooth performance in real-time rendering applications
  
      **U15**: Current tools may only generate surface geometry, while we often need volumetric meshes (e.g., VDB formats) for smoke, fire, and other complex simulations. In VFX workflows, models frequently undergo transformations such as splitting, deforming, or fracturing. Generated meshes need to be flexible and optimized for dynamic topology changes. VFX production requires ultra-detailed models with high-resolution textures (4K or higher). For example, a cracked rock might need realistic fracture details and fine texture maps for close-up shots.
  
2.  What additional features or types of generation would you like to see? For instance: dynamic mesh animations, complex scene generation, or specific material generation.

      **U1**: The ability to generate character meshes with pre-attached skeletal rigs and basic animations (e.g., breathing, walking, running) would save time and allow for quick animation testing. Support for different artistic styles, such as realistic characters, cartoon characters, or low-poly designs, to match various game art styles. The ability to generate meshes with multiple texture maps (e.g., normal maps, metallic maps, roughness maps) that align with PBR workflows, ensuring seamless integration into game engines like Unreal Engine and Unity.

      **U6**: The ability to generate entire interior scenes based on input like floor plans or simple descriptions (e.g., "a modern living room") with walls, furniture, and lighting automatically arranged. The ability to automatically determine and assign appropriate materials to objects (e.g., wood, glass, fabric) with realistic PBR parameters, or allow users to specify specific material types (e.g., marble flooring or leather couches). The tool should automatically add realistic lighting (e.g., ambient light, point lights) and provide quick preview rendering functionality to save time during visualization.

      **U15**: The ability to generate models with built-in physical properties (e.g., soft fabric, rigid metal, or glass shattering effects) to streamline integration into physics-based simulations. The ability to generate pre-fractured or deformed models, such as broken walls or bent metal, would significantly reduce manual effort in creating destruction effects. VFX artists need models to be exportable in formats compatible with industry-standard tools like Houdini or Cinema 4D (e.g., Alembic or VDB files). Additionally, cache support for animated models would be valuable for integrating complex simulations.

#### Questions about multimodal generation needs ####
* In multimodal generation tasks (e.g., generating 3D meshes from text, images, or point clouds), which input modality is the most useful for your work? Why?

     **U1: Preferred Input Mode: Image-based Input**

     We often rely on concept art or detailed reference images to guide their modeling process. Image-based input allows them to directly translate these references into 3D models, reducing the need for manual interpretation and ensuring the final output matches the visual style and proportions of the original artwork. When generating 3D characters, maintaining the intended artistic details (such as facial features, pose, or costume design) is critical. Image-based input provides a clear and direct representation of these details, which can be challenging to convey through text-based descriptions. Image-based workflows allow for quick iteration. If the generated model does not meet the requirements, artists can adjust the input image (e.g., changing proportions or adding details) and regenerate the 3D mesh, making the process highly efficient.

  Use Cases:

     * Generating a base mesh for a character from a front-facing concept art or orthographic drawings.
     * Translating stylized character designs (e.g., cartoon or anime art) into 3D models while preserving the intended aesthetic.


     **U6: Preferred Input Mode: Text-based Input**

     Text-based input enables designers to describe the desired scene in natural language (e.g., "a modern living room with a large window and wooden flooring"). This lowers the barrier for designers unfamiliar with 3D modeling tools, making the process more accessible. Text-based input allows designers to experiment with different styles and layouts quickly. For example, they can easily switch between "minimalist" and "luxurious" designs by changing the input text, which would be more time-consuming with images or manual modeling. Designers often work based on abstract ideas rather than specific visuals. Text descriptions provide the freedom to explore creative concepts without being constrained by existing reference images.

   Use Cases:

     * Quickly generating room layouts or architectural structures based on high-level descriptions.
     * Exploring diverse styles or configurations for the same space by altering the text prompts (e.g., "a Scandinavian-style bedroom" vs. "a Victorian-style bedroom").

     **U15: Preferred Input Mode: Point Cloud-based Input**

     We often work with real-world data, such as scanned environments or objects. Point cloud input provides a highly accurate representation of the geometry and spatial structure of real-world scenes, making it ideal for generating realistic 3D models. Many VFX pipelines already use point cloud data obtained from LiDAR scans, photogrammetry, or motion capture. Point cloud-based generation seamlessly integrates with these workflows, saving time and ensuring consistency between scanned data and generated 3D meshes. Point cloud input is especially useful for generating complex or irregular structures (e.g., debris, fractured objects, or organic shapes) that are difficult to describe with text or represent with images. It also allows for dynamic effects, like transforming scanned objects into destructible assets.

    Use Cases:

     * Generating a dense and accurate 3D mesh of a scanned building for destruction effects.
     * Creating a 3D model from point cloud data captured on set for seamless integration into a live-action scene.

**Design Rationale**

Rating Questions (1-9): Allow users to quantitatively evaluate specific aspects of the generation process, providing measurable insights for statistical analysis.

Open-Ended Questions: Help gather qualitative feedback on improvement areas and multimodal preferences, revealing deeper user needs and expectations.



