---
layout: default
title: Platform.FilePickerVisible
description: This will check if the file picker interface is currently visible. Some pickers will never show this, as they block the application until the picker has completed.
---
# [Platform]({{site.url}}/Pages/Reference/Platform.html).FilePickerVisible

<div class='signature' markdown='1'>
static bool FilePickerVisible{ get }
</div>

## Description
This will check if the file picker interface is
currently visible. Some pickers will never show this, as they
block the application until the picker has completed.


## Examples

### Opening a Model
This is a simple button that will open a 3D model selection
file picker, and make a call to OnLoadModel after a file has
been successfully picked!
```csharp
if (UI.Button("Open Model") && !Platform.FilePickerVisible) {
	Platform.FilePicker(PickerMode.Open, OnLoadModel, null,
		".gltf", ".glb", ".obj", ".stl", ".fbx", ".ply");
}
```
Once you have the filename, it's simply a matter of loading it
from file. This is an example of async loading a model, and
calculating a scale value that ensures the model is a reasonable
size.
```csharp
private void OnLoadModel(string filename)
{
	Task.Run(() =>
	{
		model      = Model.FromFile(filename);
		modelScale = 1 / model.Bounds.dimensions.Magnitude;
	});
}
```

