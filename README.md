# Creating GLB 3d NFTs

Create your model in a 3d program such as Blender / Maya / Cinema4d and export to a format that Unity3d can handle. (FBX, OBJ + UV Mapped Textures)


Import the file into Unity3d project
![](https://i.imgur.com/qja4N7M.png)


Configure the object, and materials. For this particular model, we used PNGs, and alpha transparecy to create the "cut out look" of the PNGs. We used the Standard Shader. For this artwork, we made copies of the transparent images, then flipped the normals to -1 zspace so that the normals faced the other way to simulate backface culling = off. This was a wrok around to using a shader that supports double sided textures.

![](https://i.imgur.com/n8tpp11.png)
![](https://i.imgur.com/SdURSUK.png)


Import plugin, PlatterGLTF Exporter, and drag a prefab of the object into the exporter. https://github.com/Plattar/gltf-exporter
![](https://i.imgur.com/22GbwDE.png)


5. Export GLTF by putting a 'prefab' into the exporter
![](https://i.imgur.com/7EnQL0X.png)

6. Unzip the GLTF file into a folder
![](https://i.imgur.com/qTbDWsi.png)

7. Use https://glb-packer.glitch.me/ by dragging the contents of folder into the web browser. This will output a 'out.glb file and ask you to save it'
![](https://i.imgur.com/2Oj5MCa.png)
![](https://i.imgur.com/5MxtHy0.png)

8. Check to see if GLB file looks right in an online browser.
https://sandbox.babylonjs.com/
![](https://i.imgur.com/ZiunZom.png)
