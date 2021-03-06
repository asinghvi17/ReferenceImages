## Axis theming

```julia
using AbstractPlotting
 using GeometryTypes

 scene = Scene()
 points = decompose(Point2f0, Circle(Point2f0(10), 10f0), 9)
 lines!(
     scene,
     points,
     linewidth = 8,
     color = :black
 )

 axis = scene[Axis] # get axis
 scene

 st = Stepper(scene, "output")
 step!(st);
 axis[:frame][:linewidth] = 5
 step!(st)
 axis[:grid][:linewidth] = (1, 5)
 step!(st)
 axis[:grid][:linecolor] = ((:red, 0.3), (:blue, 0.5))
 step!(st)
 axis[:names][:axisnames] = ("x", "y   ")
 step!(st)
 axis[:ticks][:title_gap] = 1
 step!(st)
 axis[:names][:rotation] = (0.0, -3/8*pi)
 step!(st)
 axis[:names][:textcolor] = ((:red, 1.0), (:blue, 1.0))
 step!(st)
 axis[:ticks][:font] = ("Dejavu Sans", "Helvetica")
 step!(st)
 axis[:ticks][:rotation] = (0.0, -pi/2)
 step!(st)
 axis[:ticks][:textsize] = (3, 7)
 step!(st)
 axis[:ticks][:gap] = 5
 step!(st)


```
```@raw html

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-1.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-10.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-11.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-12.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-2.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-3.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-4.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-5.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-6.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-7.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-8.jpg" alt="">

    </p>
</div>

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <img src="https://simondanisch.github.io/ReferenceImages/gallery//axis_theming/media/axis_theming-9.jpg" alt="">

    </p>
</div>

```
