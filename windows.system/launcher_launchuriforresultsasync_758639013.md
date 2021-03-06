---
-api-id: M:Windows.System.Launcher.LaunchUriForResultsAsync(Windows.Foundation.Uri,Windows.System.LauncherOptions)
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<Windows.System.LaunchUriResult> LaunchUriForResultsAsync(Windows.Foundation.Uri uri, Windows.System.LauncherOptions options)
-->

# Windows.System.Launcher.LaunchUriForResultsAsync

## -description
Asynchronously starts the default app associated with the URI scheme name for the specified URI, using the specified options.

## -parameters
### -param uri
The Uri to launch.

### -param options
The launch options.

## -returns
When this method completes, it returns the results of the launch.

## -remarks
Launching an app for results allows you to launch an app from another app and exchange data between the two.

This API must be called from within an ASTA thread (also known as a UI thread).

## -examples

## -see-also
[LaunchUriForResultsAsync(Uri, LauncherOptions, ValueSet)](launcher_launchuriforresultsasync_148601521.md), [Launch an app for results](http://msdn.microsoft.com/library/afc53d75-b3dd-4ff6-9fc0-9335242ee327)