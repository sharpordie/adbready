<hr><div>
<a href="../.."><img align="right" height="91" src="https://user-images.githubusercontent.com/72373746/202394839-d673c37b-e9a7-4c31-ad0a-04cdc9e51308.png" alt="logo"></a>
<h1>ADBREADY</h1>
<p>Android ADB Ready for Flutter</p>
</div><hr>

## `Support`

<table>
  <tr>
    <td><samp>AND</samp></td>
    <th><samp>IOS</samp></th>
    <th><samp>LIN</samp></th>
    <th><samp>MAC</samp></th>
    <th><samp>WIN</samp></th>
    <th><samp>WEB</samp></th>
  </tr>
  <tr align="center">
    <td width="50"><samp>✅</samp></td>
    <td width="50"><samp>⛔</samp></td>
    <td width="50"><samp>⛔</samp></td>
    <td width="50"><samp>⛔</samp></td>
    <td width="50"><samp>⛔</samp></td>
    <td width="50"><samp>⛔</samp></td>
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
