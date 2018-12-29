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
; Debug mode type which can be selected by user.
; on|all = All types
; off|none = Disabled debug mode
; normal = usual teraterm debug mode
; hex = hex output
; noout = disable output completely
DebugModes=all

After

; Display all characters (debug mode)
Debug=on
; Debug mode type which can be selected by user.
; on|all = All types
; off|none = Disabled debug mode
; normal = usual teraterm debug mode
; hex = hex output
; noout = disable output completely
DebugModes=hex

```

Next, you restart Tera Term and press Shift key and Escape key at the same time and turn on hexadecimal display.

By this configuration, you can see hexadecimal returned by KeiganMotor on Tera Term.

When you execute the above macro  demo_1, the log will be as follows.



