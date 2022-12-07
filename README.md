<div><hr>
<a href="../.."><img align="right" height="91" src="assets/logo.png"></a>
<h1>ADBREADY</h1>
<p>Android ADB Ready for Flutter</p>
<hr></div>

<h2><samp>OVERVIEW</samp></h2>

Provide ready to use ADB binary for Android.

<h2><samp>COVERAGE</samp></h2>

<!--
| <samp>AND</samp> | <samp>IOS</samp> | <samp>LIN</samp> | <samp>MAC</samp> | <samp>WIN</samp> | <samp>WEB</samp> |
| :-: | :-: | :-: | :-: | :-: | :-: |
| <br>✅<br><br> | <br>🚫<br><br> | <br>🚫<br><br> | <br>🚫<br><br> | <br>🚫<br><br> | <br>🚫<br><br> |
-->

<table>
  <tr>
    <th><samp>AND</samp></th>
    <th><samp>IOS</samp></th>
    <th><samp>LIN</samp></th>
    <th><samp>MAC</samp></th>
    <th><samp>WIN</samp></th>
    <th><samp>WEB</samp></th>
  </tr>
  <tr align="center">
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/9bdb4d/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ed5353/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ed5353/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ed5353/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ed5353/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ed5353/fff//?text=‏‏‎ ‎"></p></td>
  </tr>
</table>

<h2><samp>EXAMPLES</samp></h2>

### Update Package from Git

```shell
flutter pub add adbready --git-url https://github.com/sharpordie/adbready
```

### Gather ADB Path

```dart
final starter = await Adbready().deploy();
```

### Gather Product Model from Device

```dart
final address = '192.168.1.10';
final command = ['-s', address, 'shell', 'getprop ro.product.model'];
final process = await Adbready().invoke(command)
final product = process.stdout;
```

<hr>
