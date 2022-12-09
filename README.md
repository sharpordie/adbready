# <samp>ADBREADY</samp>

Provides ready to use ADB binary for Android.

<!--
## <samp>PREFACE</samp></h2>
## <samp>PREVIEW</samp></h2>
## <samp>STARTER</samp></h2>
-->

DEVICES  
PREVIEW  
SYSTEMS  
FACTORS  
PREFACE  

| <samp>AND</samp> | <samp>IOS</samp> | <samp>LIN</samp> | <samp>MAC</samp> | <samp>WIN</samp> | <samp>WEB</samp> |
| :-: | :-: | :-: | :-: | :-: | :-: |
| <br>🟩<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> |

## <samp>PREVIEW</samp></h2>

### Update Package from Git

```shell
flutter pub add adbready --git-url https://github.com/sharpordie/adbready
```

### Gather ADB Path

```dart
final starter = await Adbready().deploy();
```

### Invoke ADB Command

```dart
final address = '192.168.1.10';
final command = ['-s', address, 'shell', 'getprop ro.product.model'];
final process = await Adbready().invoke(command)
final product = process.stdout;
```
