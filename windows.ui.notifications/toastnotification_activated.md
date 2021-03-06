---
-api-id: E:Windows.UI.Notifications.ToastNotification.Activated
-api-type: winrt event
---

<!-- Event syntax
public event Windows.Foundation.TypedEventHandler Activated<Windows.UI.Notifications.ToastNotification,  object>
-->

# Windows.UI.Notifications.ToastNotification.Activated

## -description
Occurs when user activates a toast notification through a click or touch. Apps that are running subscribe to this event
<!-- @WRITER erictill 10/26/2011 : and call <xref rid="w_ui_notif.toastactivatedeventhandler" targtype="delegate">ToastActivatedEventHandler</xref> in response -->
.

## -remarks
In the case of toast raised by a desktop app, that app must subscribe to at least the [Activated](toastnotification_activated.md) event so that it can handle the expected activation of the app from the toast when the user selects it.

## -examples

## -see-also
[Toast notifications sample](http://go.microsoft.com/fwlink/p/?linkid=231503), [Sending toast notifications from desktop apps sample](http://go.microsoft.com/fwlink/p/?linkid=231503), [Toast XML schema](XREF:TODO:toast.Schema_Root), [Tiles, badges, and notifications](http://msdn.microsoft.com/library/48ee4328-7999-40c2-9354-7ea7d488c538), [Quickstart: Sending a toast notification](http://msdn.microsoft.com/library/098df37c-4d40-4499-b809-ccb651da1cba), [Quickstart: Sending a toast push notification](XREF:TODO:m_ui_tiles.quickstart_sending_a_toast_push), [Quickstart: Sending a toast notification from the desktop](http://msdn.microsoft.com/library/1d20ed75-e24a-4e60-91ab-cfcbe902a68e), [Guidelines and checklist for toast notifications](XREF:TODO:m_ui_tiles.guidelines_and_checklist_for_toast), [How to handle activation from a toast notification](http://msdn.microsoft.com/library/74ba3513-0a52-46a0-8769-ed58abe7c05a), [How to opt in for toast notifications](http://msdn.microsoft.com/library/809cdd36-6de1-4de0-88b2-62b46cafdb28), [How to schedule a toast notification](http://msdn.microsoft.com/library/18a09413-1679-4606-8175-346f4fe6a4f8), [How to enable desktop toast notifications through an AppUserModelID](http://msdn.microsoft.com/library/bb32cd0a-99e6-47dc-a913-39a7b3027314), [The toast template catalog](http://msdn.microsoft.com/library/1a437614-4259-426b-8e3f-ca57368b2e7a), [Toast audio options](http://msdn.microsoft.com/library/12185879-1f9b-4bdc-99e7-a6f2f62806cb)