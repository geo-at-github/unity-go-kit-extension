# unity-go-kit-extension
My extensions for the GoKit tween library for Unity 3D (https://github.com/prime31/GoKit).
It contains tweens for achorPositions (tween all four anchors relative to their "center") and the anchored position (http://docs.unity3d.com/ScriptReference/RectTransform-anchoredPosition.html).

It is implemented with c# extension methods to GoKit (https://msdn.microsoft.com/en-us/library/bb383977.aspx).


Usage
-----
Usage is similar to the translation tweens on GoKit.
The target object needs to have a RectTransform.

Import the extension with ```using GeosGoKitExtension;```

anchorPositions(this GoTweenConfig goTweenConfig, Vector2 endValue, bool isRelative = false)
```
Vector2 targetPos = new Vector2( 0.0f, 0.0f);
var anchorPositionsTween = new GoTween(your2dObject.transform, 1.0f, new GoTweenConfig().anchorPositions(targetPos, false));
```

anchoredPosition(this GoTweenConfig goTweenConfig, Vector2 endValue, bool isRelative = false)
```
Vector2 targetPos = new Vector2( 0.0f, 0.0f);
var anchorPositionsTween = new GoTween(your2dObject.transform, 1.0f, new GoTweenConfig().anchoredPosition(targetPos, false));
```

Installation
-----
Simply add the folder to your script assets in Unity.