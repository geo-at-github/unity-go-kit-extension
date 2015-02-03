# unity-go-kit-extension
My extensions for the GoKit tween llibrary for Unity 3D.
It contains tweens for achorPositions (tween all four anchors relative to their "center") and the anchored position (http://docs.unity3d.com/ScriptReference/RectTransform-anchoredPosition.html).

Usage
-----
Usage is similar to the translation tweens on GoKit.
The target object needs to have a RectTransform.

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