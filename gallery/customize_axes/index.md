## Customize Axes

```julia
using AbstractPlotting

 x = LinRange(0,3pi,200); y = sin.(x)
 lin = lines(x, y, padding = (0.0, 0.0), axis = (
     names = (axisnames = ("", ""),),
     grid = (linewidth = (0, 0),),
 ))


```
```@raw html

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//customize_axes/media/image.jpg" alt="">

    </p>
</div>

```
