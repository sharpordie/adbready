<hr><div>
<a href="../.."><img align="right" height="91" src="https://user-images.githubusercontent.com/72373746/202394839-d673c37b-e9a7-4c31-ad0a-04cdc9e51308.png" alt="logo"></a>
<h1>adbready</h1>
<p>Android ADB ready for Flutter</p>
</div><hr>

## `Support`

<table>
  <tr>
    <th>AND</th>
    <th>IOS</th>
    <th>LIN</th>
    <th>MAC</th>
    <th>WIN</th>
  </tr>
  <tr align="center">
    <td width="65"><p><br><img src="https://fakeimg.pl/35x35/d1ff82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="65"><p><br><img src="https://fakeimg.pl/35x35/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="65"><p><br><img src="https://fakeimg.pl/35x35/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="65"><p><br><img src="https://fakeimg.pl/35x35/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
    <td width="65"><p><br><img src="https://fakeimg.pl/35x35/ff8c82/fff//?text=‏‏‎ ‎"></p></td>
  </tr>
</table>

## `Install`

```shell
flutter pub add adbready --git-url https://github.com/sharpordie/adbready
```

## `Samples`

### Gather ADB Path

```dart
final starter = await Adbready().deploy();
```

### Gather External Device Product Model

```dart
final address = '192.168.1.10'; // Address of the target device.
final command = ['-s', address, 'shell', 'getprop ro.product.model'];
final process = await Adbready().invoke(command)
final product = process.stdout;
```