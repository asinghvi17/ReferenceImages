## Tutorial linesegments

```julia
using AbstractPlotting

 points = [
     Point2f0(0, 0) => Point2f0(5, 5);
     Point2f0(15, 15) => Point2f0(25, 25);
     Point2f0(0, 15) => Point2f0(35, 5);
     ]
 scene = linesegments(points, color = :red, linewidth = 2)


```
```@raw html

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//tutorial_linesegments/media/image.jpg" alt="">

    </p>
</div>

```
