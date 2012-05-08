---
layout: post
title: "MT4 Keyboard Shortcuts"
date: 2012-05-08 22:27
comments: false
categories: ['trading','forex','MT4']
---

This post lists MT4 keyboard shortcuts, as sometimes it is a pain to swap between mouse and keyboard. 

<!-- more -->

## Scroll

{% codeblock %}
Left            : Left
Left Fast       : Page Up 
Left OneBar     : F12
Right           : Right
Right Fast      : Page Down
Right OneBar    : Shift+F12
End             : End
Start           : Home
{% endcodeblock %}

## Windows
{% codeblock %}
Data            : Ctrl+D
Indicators      : Ctrl+I
Market Watch    : Ctrl+M
Navigator       : Ctrl+N
Terminal        : Ctrl+T
Tester          : Ctrl+R
{% endcodeblock %}

## Switch
{% codeblock %}
Chart Next      : Ctrl+F6
Profile Next    : Ctrl+F5
{% endcodeblock %}

## Dialogs
{% codeblock %}
Chart Props     : F8
Global Vars     : F3
History Center  : F2
New Order       : F9
Open Windows    : Alt+W
Options         : Ctrl+O
Prices Dialog   : F10
Print           : Ctrl+P
{% endcodeblock %}

## Toggle
{% codeblock %}
Bar Chart       : Alt+1
Candle Chart    : Alt+2
Fast Nav        : Enter
Full screen     : F11
Grid            : Ctrl+G
Line Chart      : Alt+3
OHLC            : Ctrl+H
Period Seps     : Ctrl+Y
Volume          : Ctrl+L
{% endcodeblock %}

## Miscellany
{% codeblock %}
Close Dialogs   : Esc
Close Window    : Ctrl+F4
Copy            : Ctrl+C
Crosshair       : Ctrl+F
Help            : F1
MetaEditor      : F4
Quit            : Alt+F4
Save            : Ctrl+S
Undo            : Ctrl+Z
Zoom In         : +
Zoom out        : -
{% endcodeblock %}

There is no facility within MT4 to assign keyboard shortcuts. But if you want to expand the range of keyboard shortcuts then you can use a free utility called [AutoHotKey][001], you can then go crazy with keyboard shortcuts.  I found this basic AutoHotKey script for MT4 somewhere. Thanks to the anonymous user. 

{% codeblock %}
;# = Windows Key
;^ = Control
;! = Alt
;+ = Shift 
;Demo Script

CapsLock & c::run, calc.exe

;FXDD MT4 Scripts

;TIMEFRAMES

CAPSLOCK & 1::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}M1{ENTER}
return

CAPSLOCK & 2::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}M5{ENTER}
return

CAPSLOCK & 3::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}M15{ENTER}
return

CAPSLOCK & 4::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}M30{ENTER}
return

CAPSLOCK & 5::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}H1{ENTER}
return

CAPSLOCK & 6::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}H4{ENTER}
return

CAPSLOCK & 7::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}D1{ENTER}
return

CAPSLOCK & 8::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}WEEKLY{ENTER}
return

CAPSLOCK & 9::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}MN{ENTER}
return

;TEMPLATES

CAPSLOCK & q::
send, {ALT}CT{Down}{Down}{Down}{ENTER}{END}
return
    
CAPSLOCK & w::
send, {ALT}CT{Down}{Down}{Down}{Down}{ENTER}{END}
return

CAPSLOCK & e::
send, {ALT}CT{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return

CAPSLOCK & r::
send, {ALT}CT{Down}{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return

CAPSLOCK & t::
send, {ALT}CT{Down}{Down}{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return

CAPSLOCK & y::
send, {ALT}CT{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return
;PAIRS

CAPSLOCK & A::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}EURUSD{ENTER}
return

CAPSLOCK & S::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}GBPUSD{ENTER}
return
    
CAPSLOCK & D::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}GBPJPY{ENTER}
return
    
CAPSLOCK & F::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}USDJPY{ENTER}
return
    
CAPSLOCK & G::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}AUDUSD{ENTER}
return
    
CAPSLOCK & H::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}USDCAD{ENTER}
return
    
CAPSLOCK & J::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}EURGBP{ENTER}
return

CAPSLOCK & K::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}USDCHF{ENTER}
return

CAPSLOCK & L::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}EURJPY{ENTER}
return

CAPSLOCK & M::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}EURCHF{ENTER}
return
    
CAPSLOCK & N::
send, {ESC}{ENTER}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}{BS}CHFJPY{ENTER}
return
;MISC
;TOGGLE FOREGROUND
CAPSLOCK & Z::
send, {ALT}C{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return

;TOGGLE CHART SCROLL
CAPSLOCK & X::
send, {ALT}C{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return
    
;CHART SHIFT
CAPSLOCK & V::
send, {ALT}C{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{Down}{ENTER}{END}
return

{% endcodeblock %}

[001]:http://www.autohotkey.com/
