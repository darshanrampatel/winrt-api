---
-api-id: T:Windows.UI.Xaml.Controls.BitmapIcon
-api-type: winrt class
---

<!-- Class syntax.
public class BitmapIcon : Windows.UI.Xaml.Controls.IconElement, Windows.UI.Xaml.Controls.IBitmapIcon
-->

# Windows.UI.Xaml.Controls.BitmapIcon

## -description
Represents an icon that uses a bitmap as its content.

## -xaml-syntax
```xaml
<BitmapIcon .../>
```


## -remarks
To use a [BitmapIcon](bitmapicon.md) as the [Icon](appbarbutton_icon.md) for an [AppBarButton](appbarbutton.md), you specify the URI of an image file.

The file that you use should be a solid image on a transparent background. The bitmap image as retrieved from the [UriSource](bitmapicon_urisource.md) location is expected to be a true bitmap that has transparent pixels and non-transparent pixels. The recommended format is PNG. Other file-format image sources will load apparently without error but result in a solid block of the foreground color inside the [AppBarButton](appbarbutton.md).

All color info is stripped from the bitmap when the [BitmapIcon](bitmapicon.md) renders in an [AppBarButton](appbarbutton.md). The remaining non-transparent colors are combined to produce an image that's entirely the foreground color as set by the [Foreground](iconelement_foreground.md) property (this typically comes from styles or templates, such as the default template resolving to a theme resource).

You typically specify a [UriSource](bitmapicon_urisource.md) value that references a bitmap that you've included as part of the app, as a resource or otherwise within the app package. For more info on the **ms-appx:** scheme and other URI schemes that you can use to reference resources in your app, see [Uri schemes](http://msdn.microsoft.com/library/f3b3ae74-aaea-4f00-8f0a-4c231b8745af).

> [!NOTE]
> You can set the **Foreground** property on the [AppBarButton](appbarbutton.md) or on the [BitmapIcon](bitmapicon.md). If you set the [Foreground](control_foreground.md) on the [AppBarButton](appbarbutton.md), it's applied only to the default visual state. It's not applied to the other visual states defined in the [AppBarButton](appbarbutton.md) template, like `MouseOver`. If you set the [Foreground](iconelement_foreground.md) on the [BitmapIcon](bitmapicon.md), the color is applied to all visual states.

## -examples
This example shows an [AppBarButton](appbarbutton.md) with a [BitmapIcon](bitmapicon.md). The [UriSource](bitmapicon_urisource.md) specifies an image that's included in the app package.

```xaml
<AppBarButton Label="BitmapIcon" Click="AppBarButton_Click">
    <AppBarButton.Icon>
        <BitmapIcon UriSource="ms-appx:///Assets/globe.png"/>
    </AppBarButton.Icon>
</AppBarButton>
```



## -see-also
[IconElement](iconelement.md), [AppBarButton](appbarbutton.md), [AppBarToggleButton](appbartogglebutton.md), [FontIcon](fonticon.md), [PathIcon](pathicon.md), [SymbolIcon](symbolicon.md), [Controls list](http://msdn.microsoft.com/library/11172840-a63d-4f48-9db4-7baca06308ee), [Controls by function](http://msdn.microsoft.com/library/8db4347b-91d6-4659-91f2-80ecf7bbb596)