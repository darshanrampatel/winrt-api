---
-api-id: T:Windows.UI.Xaml.Controls.Primitives.RepeatButton
-api-type: winrt class
---

<!-- Class syntax.
public class RepeatButton : Windows.UI.Xaml.Controls.Primitives.ButtonBase, Windows.UI.Xaml.Controls.Primitives.IRepeatButton
-->

# Windows.UI.Xaml.Controls.Primitives.RepeatButton

## -description
Represents a control that raises its [Click](buttonbase_click.md) event repeatedly when it is pressed and held.

## -xaml-syntax
```xaml
<RepeatButton .../>
-or-
<RepeatButton>
    singleObject
</RepeatButton>
-or-
<RepeatButton ...>stringContent</RepeatButton>
```


## -remarks
A [RepeatButton](repeatbutton.md) is a button that raises [Click](buttonbase_click.md) events repeatedly from the time it is pressed until it is released. Set the [Delay](repeatbutton_delay.md) property to specify the time that the [RepeatButton](repeatbutton.md) waits after it is pressed before it starts repeating the click action. Set the [Interval](repeatbutton_interval.md) property to specify the time between repetitions of the click action. Times for both properties are specified in milliseconds.

## -examples
The following example shows two [RepeatButton](repeatbutton.md) controls whose respective [Click](buttonbase_click.md) events are used to increase and decrease the value shown in a [TextBlock](../windows.ui.xaml.controls/textblock.md).

```csharp
<StackPanel>
    <RepeatButton Width="100" Delay="500" Interval="100" Click="Increase_Click">Increase</RepeatButton>
    <RepeatButton Width="100" Delay="500" Interval="100" Click="Decrease_Click">Decrease</RepeatButton>
    <TextBlock x:Name="clickTextBlock" Text="Number of Clicks:"/>
</StackPanel>
```

```csharp
private static int _clicks = 0;
private void Increase_Click(object sender, RoutedEventArgs e)
{
    _clicks += 1;
    clickTextBlock.Text = "Number of Clicks: " + _clicks;
}

private void Decrease_Click(object sender, RoutedEventArgs e)
{
    if(_clicks > 0)
    {
        _clicks -= 1;
        clickTextBlock.Text = "Number of Clicks: " + _clicks;
    }
}
```


<!--<auto_snippet sample_id="System.Windows.Controls.RepeatButtonEx" snippet_id="1"/>
        <auto_snippet sample_id="System.Windows.Controls.RepeatButtonEx" snippet_id="11"/>-->

## -see-also
[ButtonBase](buttonbase.md)