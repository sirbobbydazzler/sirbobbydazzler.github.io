---
title: Rox Camera Provider
description: Rox Tools for .Net by AiRoBo Software
---
Rox Camera Provider acquires images with the device camera using native platform components.

*Rox Camera Provider for Xamarin.Forms supports Android, iOS, and UWP*.

The Rox Camera Provider has the following methods:

```csharp
    //Take a picture with the device camera
    Task<ImageSource> AcquirePicture();
```

## Platform Considerations

### Android

In your Android project `MainActivity.cs` code file, you must call `Rox.Camera.Init(Activity)` before `Xamarin.Forms.Forms.Init()`. It should look something like:

```csharp
    global::Rox.Camera.Init(this);

    global::Xamarin.Forms.Forms.Init();

    LoadApplication(new MyCameraApplication());
```

### iOS

In your iOS project `AppDelegate.cs` code file, you must call `Rox.Camera.Init()` before `Xamarin.Forms.Forms.Init()`. It should look something like:

```csharp
    global::Rox.Camera.Init();

    global::Xamarin.Forms.Forms.Init();

    LoadApplication(new MyCameraApplication());
```

### Links

| Site | URL |
| --- | --- |
| Help | [rox.tools/control/camera](https://rox.tools/control/camera/) |
| | [rox.tools/control/camera/xamarin](https://rox.tools/control/camera/xamarin/) |
| Sample | [rox.gallery/control](https://rox.gallery/control/) |
| Source | [github.com/ai-ro-bo/Rox.Control.Camera.Xamarin](https://github.com/ai-ro-bo/Rox.Control.Camera.Xamarin) |
| NuGet | [nuget.org/packages/Rox.Xamarin.Camera](https://www.nuget.org/packages/Rox.Xamarin.Camera/) |
| AiRoBo | [airobo.software](https://airobo.software/) |

| Site | [rox.tools/control/camera](https://rox.tools/control/camera/) |
| NuGet | [nuget.org/packages/Rox.Xamarin.Camera](https://www.nuget.org/packages/Rox.Xamarin.Camera/) |
| Source | [github.com/ai-ro-bo/Rox.Control.Camera.Xamarin](https://github.com/ai-ro-bo/Rox.Control.Camera.Xamarin) |

---
Visit [*`AiRoBo Software`*](https://airobo.software/) for more information.
