# Windows下一键交换Esc和caps和一键恢复的方法

### 1、交换Esc和caps的方法

将如下内容保存到.reg文件，双击运行后重启即可

```
Windows Registry Editor Version 5.00
 
[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout]
"Scancode Map"=hex:00,00,00,00,00,00,00,00,03,00,00,00,3a,00,01,00,01,00,3a,00,00,00,00,00
```

----

### 2、恢复默认Esc和caps的方法

将如下内容保存到.reg文件，双击运行后重启即可

```
Windows Registry Editor Version 5.00
 
[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Keyboard Layout]
"Scancode Map"=-
```

----