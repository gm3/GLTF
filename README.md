# Creating GLB 3d NFTs Using Platter Exporter and Unity3d

1. Create your model in a 3d program such as Blender / Maya / Cinema4d and export to to a format that Unity3d can handle. (FBX, OBJ + UV Mapped Textures)


2. Import the file into Unity3d project
![](https://i.imgur.com/qja4N7M.png)


3. Configure the object, and materials. For this particular model, we used PNGs, and alpha transparecy to create the "cut out look" of the PNGs. We used the Standard Shader
For this artwork, we made copies of the transparent images, then flipped the normals to -1 zspace so that the normals faced the other way to simulate backface culling = off. This was a wrok around to using a shader that supports double sided textures.


4. Import plugin, PlatterGLTF Exporter, and drag a prefab of the object into the exporter. https://github.com/Plattar/gltf-exporter
5. ![](https://i.imgur.com/22GbwDE.png)



5. Export GLTF by putting a 'prefab' into the exporter


6. ![](https://i.imgur.com/7EnQL0X.png)

7. Unzip the GLTF file into a folder
![](https://i.imgur.com/qTbDWsi.png)
8. Use https://glb-packer.glitch.me/ by dragging the contents of folder into the web browser. This will output a 'out.glb file and ask you to save it'
![](https://i.imgur.com/2Oj5MCa.png)

9. Check to see if GLB file looks right in an online browser.
https://sandbox.babylonjs.com/
![](https://i.imgur.com/ZiunZom.png)
