PhoneGap Custom URL Scheme Plugin
=================================

Use Custom URL Schemes in a PhoneGap application. You don't need this plugin to do that but it handles the config changes which is useful when you're using the new Cordova CLI tool and you don't want to edit the contents of the platforms folder directly.

Install using the cordova CLI:

```
cordova plugin add https://github.com/almost/pgit inithonegap-urlscheme-plugin.git --variable
URLSCHEME="myscheme"
```

Only support iOS for obvious reasons.

To use put the following JavaScript function on your main page (this is from regular PhoneGap, no actual code is added by this plugin)

```
function handleOpenURL(url) {
  // Do something with the custom url scheme
}
```
