---
-api-id: M:Windows.UI.Input.Inking.InkStrokeBuilder.EndStroke(Windows.UI.Input.PointerPoint)
-api-type: winrt method
---

<!-- Method syntax
public Windows.UI.Input.Inking.InkStroke EndStroke(Windows.UI.Input.PointerPoint pointerPoint)
-->

# Windows.UI.Input.Inking.InkStrokeBuilder.EndStroke

## -description
Stops building the ink stroke.

> [!NOTE]
> [EndStroke](inkstrokebuilder_endstroke.md) is not supported by [InkPresenter](inkpresenter.md). Use [CreateStrokeFromInkPoints](inkstrokebuilder_createstrokefrominkpoints.md) and [SetDefaultDrawingAttributes](inkstrokebuilder_setdefaultdrawingattributes.md) to programmatically build strokes for an [InkPresenter](inkpresenter.md).

## -parameters
### -param pointerPoint
The last point for the stroke.

## -returns
The stroke built from the points.

## -remarks

## -examples

## -see-also
[Pen and stylus interactions](http://msdn.microsoft.com/library/3da4f2d2-5405-42a1-9ed9-3a87bcd84c43), [Ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620308), [Simple ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620312), [Complex ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620314)