## Mouse Picking

```julia
using AbstractPlotting

 img = rand(100, 100)
 scene = Scene(resolution = (500, 500))
 heatmap!(scene, img, scale_plot = false)
 clicks = Node(Point2f0[(0,0)])
 on(scene.events.mousebuttons) do buttons
    if ispressed(scene, Mouse.left)
        pos = to_world(scene, Point2f0(scene.events.mouseposition[]))
        push!(clicks, push!(clicks[], pos))
    end
    return
 end
 scatter!(scene, clicks, color = :red, marker = '+', markersize = 10)
 RecordEvents(scene, "output")


```
```@raw html

<div style="display:inline-block">
    <p style="display:inline-block; text-align: center">
        <video controls autoplay loop muted>
  <source src="https://simondanisch.github.io/ReferenceImages/gallery//mouse_picking/media/video.mp4" type="video/mp4">
  Your browser does not support mp4. Please use a modern browser like Chrome or Firefox.
</video>

    </p>
</div>

```
