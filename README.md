<hr><div>
<a href="../.."><img align="right" height="91" src="https://user-images.githubusercontent.com/72373746/202394839-d673c37b-e9a7-4c31-ad0a-04cdc9e51308.png" alt="logo"></a>
<h1>ADBREADY</h1>
<p>Android ADB Ready for Flutter</p>
</div><hr>

## PREFACE

Library providing the ADB binary compiled for Android.

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
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/d1ff82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="55"><p><br><img src="https://fakeimg.pl/30x30/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
  </tr>
</table>

## PREVIEW

### Install Package from Git

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
