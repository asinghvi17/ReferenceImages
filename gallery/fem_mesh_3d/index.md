## FEM mesh 3D

```julia
using AbstractPlotting
 using GeometryTypes, GLMakie

 cat = GLMakie.loadasset("cat.obj")
 vertices = decompose(Point3f0, cat)
 faces = decompose(Face{3, Int}, cat)
 coordinates = [vertices[i][j] for i = 1:length(vertices), j = 1:3]
 connectivity = [faces[i][j] for i = 1:length(faces), j = 1:3]
 mesh(
     coordinates, connectivity,
     color = rand(length(vertices))
 )


```
```@raw html

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//fem_mesh_3d/media/image.jpg" alt="">

    </p>
</div>

```
