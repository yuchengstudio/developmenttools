# 如何让tera term显示HEX码

Display HEX with Tera Term

KeiganMotor echos received bytes array.
This function may be deprecated and change to more readable logging function in the future .

Tera Term can display hexadecimal after the following configuration. 

You edit TERATERM.INI in the Tera Term installed directory. In most cases, it will be in C:\Program Files (x86)\teraterm.

Before
```
; Display all characters (debug mode)
Debug=off

; Delimters for word selection
;  (compatible with earlier versions of Tera Term)
;  DelimList=$20
;  DelimDBCS=off
DelimList=$20!"#$24%&'()*+,:;<=>?@[\]^`{|}
DelimDBCS=on

After

; Display all characters (debug mode)
Debug=on

; Delimters for word selection
;  (compatible with earlier versions of Tera Term)
;  DelimList=$20
;  DelimDBCS=off
DelimList=$20!"#$24%&'()*+,:;<=>?@[\]^`{|}
DelimDBCS=on

```
然后重启tera term, 使用 shift + ESC 组合件切换显示模式，有时需要切换2次，直到显示HEX码为止



