<!--
<div><hr>
<a href="../.."><img align="right" height="91" src="assets/logo.png"></a>
<h1>ADBREADY</h1>
<p>Android ADB Ready for Flutter</p>
<hr></div>

## <samp>FUNDINGS</samp>

<a href="../.." target="_blank"><img src="https://raw.githubusercontent.com/sharpordie/mybadges/main/src/kofi.svg"></a>
-->

# <samp>ADBREADY</samp>

Provides ready to use ADB binary for Android.

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
