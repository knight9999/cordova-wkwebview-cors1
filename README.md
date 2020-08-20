# Cordova 5.1.1 + WKWebView (Xcode 11.3)

Add following in config.xml 

```
    <preference name="WKWebViewOnly" value="true"/>
    <preference name="CordovaWebViewEngine" value="CDVWKWebViewEngine"/>
    <feature name="CDVWKWebViewEngine">
      <param name="ios-package" value="CDVWKWebViewEngine"/>
    </feature>
```

Remove following in config.xml 

```
    <preference name="scheme" value="app" />
    <preference name="hostname" value="localhost" />
```

Set Configure -> App Settings for iOS

Set WkWebView

Set Build -> Build Environemnt Settings in menu.

Select Cordova 5.1.1

# Cordova 6.1.0 + Default WebView (= WKWebView)  (Xcode 11.3)

Remove following in config.xml

```
    <preference name="WKWebViewOnly" value="true"/>
    <preference name="CordovaWebViewEngine" value="CDVWKWebViewEngine"/>
    <feature name="CDVWKWebViewEngine">
      <param name="ios-package" value="CDVWKWebViewEngine"/>
    </feature>
```

Remove following in config.xml

```
    <preference name="scheme" value="app" />
    <preference name="hostname" value="localhost" />
```

Set Configure -> App Settings for iOS

Set UIWebView
(This UIWebView means no additional WKWebView. Therefore the default webview which is WKWebivew in this case is used.)


Set Build -> Build Environemnt Settings in menu.

Select Cordova 6.1.0


# Cordova 6.1.0 +  Default WebView (= WKWebView) + Custom scheme (Xcode 11.3)

Remove following in config.xml

```
    <preference name="WKWebViewOnly" value="true"/>
    <preference name="CordovaWebViewEngine" value="CDVWKWebViewEngine"/>
    <feature name="CDVWKWebViewEngine">
      <param name="ios-package" value="CDVWKWebViewEngine"/>
    </feature>
```

Add following in config.xml

```
    <preference name="scheme" value="app" />
    <preference name="hostname" value="localhost" />
```

Set UIWebView
(This UIWebView means no additional WKWebView. Therefore the default webview which is WKWebivew in this case is used.)


Set Build -> Build Environemnt Settings in menu.

Select Cordova 6.1.0

