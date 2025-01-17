---
layout: default
title: UI.SetElementVisual
description: Override the visual assets attached to a particular UI element.  Note that StereoKit's default UI assets use a type of quadrant sizing that is implemented in the Material _and_ the Mesh. You don't need to use quadrant sizing for your own visuals, but if you wish to know more, you can read more about the technique [here](https.//playdeck.net/blog/quadrant-sizing-efficient-ui-rendering). You may also find UI.QuadrantSizeVerts and UI.QuadrantSizeMesh to be helpful.
---
# [UI]({{site.url}}/Pages/Reference/UI.html).SetElementVisual

<div class='signature' markdown='1'>
static void SetElementVisual([UIVisual]({{site.url}}/Pages/Reference/UIVisual.html) visual, [Mesh]({{site.url}}/Pages/Reference/Mesh.html) mesh, [Material]({{site.url}}/Pages/Reference/Material.html) material)
</div>

|  |  |
|--|--|
|[UIVisual]({{site.url}}/Pages/Reference/UIVisual.html) visual|Which UI visual element to override.|
|[Mesh]({{site.url}}/Pages/Reference/Mesh.html) mesh|The Mesh to use for the UI element's visual             component. The Mesh will be scaled to match the dimensions of the             UI element.|
|[Material]({{site.url}}/Pages/Reference/Material.html) material|The Material to use when rendering the UI             element. The default Material is specifically designed to work             with quadrant sizing formatted meshes.|

Override the visual assets attached to a particular UI
element.

Note that StereoKit's default UI assets use a type of quadrant
sizing that is implemented in the Material _and_ the Mesh. You
don't need to use quadrant sizing for your own visuals, but if
you wish to know more, you can read more about the technique
[here](https://playdeck.net/blog/quadrant-sizing-efficient-ui-rendering).
You may also find UI.QuadrantSizeVerts and UI.QuadrantSizeMesh to
be helpful.



