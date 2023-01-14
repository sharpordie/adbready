# <samp>OVERVIEW</samp>

| <samp>AND</samp> | <samp>IOS</samp> | <samp>LIN</samp> | <samp>MAC</samp> | <samp>WIN</samp> | <samp>WEB</samp> |
| :-: | :-: | :-: | :-: | :-: | :-: |
| <br>🟩<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> | <br>🟥<br><br> |

# <samp>GUIDANCE</samp>

## Update package from git

```shell
flutter pub add adbready --git-url https://github.com/sharpordie/adbready
```

## Gather executable path

```dart
final starter = await Adbready().deploy();
```

## Invoke command to target

```dart
final address = '192.168.1.10';
final command = ['-s', address, 'shell', 'getprop ro.product.model'];
final process = await Adbready().invoke(command)
final product = process.stdout;
```
