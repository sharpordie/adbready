# <samp>ADBREADY</samp>

Provides ready to use ADB binary for Android.

## <samp>DEVICES</samp></h2>
## <samp>PREFACE</samp></h2>
## <samp>PREVIEW</samp></h2>
## <samp>TARGETS</samp></h2>
## <samp>STARTER</samp></h2>
## <samp>###</samp></h2>
## <samp>SYSTEMS</samp></h2>
## <samp>SAMPLES</samp></h2>
## <samp>EXAMPLE</samp></h2>
## <samp>RUNNING</samp></h2>
## <samp>TARGETS</samp></h2>
## <samp>SUPPORT</samp></h2>
## <samp>###</samp></h2>
## <samp>GALLERY</samp></h2>
## <samp>STARTER</samp></h2>
## <samp>SPARKLE</samp></h2>
## <samp>###</samp></h2>
## <samp>STARTING</samp></h2>
## <samp>PICTURES</samp></h2>
## <samp>ADDITION</samp></h2>
## <samp>GUIDANCE</samp></h2>
## <samp>###</samp></h2>
## ~~<samp>ADDENDUM</samp></h2>~~
## <samp>COVERAGE</samp></h2>

| <samp>AND</samp> | <samp>IOS</samp> | <samp>LIN</samp> | <samp>MAC</samp> | <samp>WIN</samp> | <samp>WEB</samp> |
| :-: | :-: | :-: | :-: | :-: | :-: |
| <br>🟩<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> |

## <samp>EXAMPLES</samp></h2>

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
