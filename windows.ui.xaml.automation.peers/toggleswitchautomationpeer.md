---
-api-id: T:Windows.UI.Xaml.Automation.Peers.ToggleSwitchAutomationPeer
-api-type: winrt class
---

<!-- Class syntax.
public class ToggleSwitchAutomationPeer : Windows.UI.Xaml.Automation.Peers.FrameworkElementAutomationPeer, Windows.UI.Xaml.Automation.Peers.IToggleSwitchAutomationPeer, Windows.UI.Xaml.Automation.Provider.IToggleProvider
-->

# Windows.UI.Xaml.Automation.Peers.ToggleSwitchAutomationPeer

## -description
Exposes [ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md) types to Microsoft UI Automation.

## -remarks
The Windows Runtime  [ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md) class creates a new [ToggleSwitchAutomationPeer](toggleswitchautomationpeer.md) as its [OnCreateAutomationPeer](../windows.ui.xaml/uielement_oncreateautomationpeer.md) definition. [ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md) is sealed, so the normal scenario of deriving from the [ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md) class and its existing peer isn't applicable to [ToggleSwitchAutomationPeer](toggleswitchautomationpeer.md).

### Default peer implementation and overrides in **ToggleSwitchAutomationPeer**

[ToggleSwitchAutomationPeer](toggleswitchautomationpeer.md) has overrides of **Core** methods such that the associated [AutomationPeer](automationpeer.md) methods provide peer-specific information to a Microsoft UI Automation client.

+ [GetPattern](automationpeer_getpattern.md) reports that the peer provides pattern support for [PatternInterface.Toggle](patterninterface.md) ([IToggleProvider](../windows.ui.xaml.automation.provider/itoggleprovider.md)).
+ [GetClassName](automationpeer_getclassname.md) returns "ToggleSwitch".
+ [GetAutomationControlType](automationpeer_getautomationcontroltype.md) returns [AutomationControlType.Button](automationcontroltype.md).
+ [GetLocalizedControlType](automationpeer_getlocalizedcontroltype.md) returns a localized resource string. This is usually handled in [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md) but [ToggleSwitchAutomationPeer](toggleswitchautomationpeer.md) has its own implementation.
This peer raises toggle-related automation events on behalf of its owner class.

Although a [ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md) can have text content, there is no [GetName](automationpeer_getname.md) implementation that can use a string representation. You should set a value for automation **Name** using the [AutomationProperties](../windows.ui.xaml.automation/automationproperties.md) attached properties.

The peer also has other behaviors that are provided by the base [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md) class. For more info, see "Base implementation in FrameworkElementAutomationPeer" section of [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4).

## -examples

## -see-also
[ToggleSwitch](../windows.ui.xaml.controls/toggleswitch.md), [FrameworkElementAutomationPeer](frameworkelementautomationpeer.md), [IToggleProvider](../windows.ui.xaml.automation.provider/itoggleprovider.md), [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4)