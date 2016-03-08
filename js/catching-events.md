#Catching Events on Console

Instead of using Chrome Dev Tool to catch event, which I don't know how it works at the momment, events can be catched using function `monitorEvents` on console

##Usage

$0 is current DOM element, catch every events happening on $0
```
monitorEvents($0)
monitorEvents(document.body)
```

catch one event in particular
```
monitorEvents($0,'keyup')
```

catch multiple events
```
monitorEvents($0,'keydown')
monitorEvents($0,'keypress')
```

##List of catchable events
```
mouse:  “mousedown”, “mouseup”, “click”, “dblclick”, “mousemove”, “mouseover”, “mouseout”, “mousewheel”
key: “keydown”, “keyup”, “keypress”, “textInput”
touch:  “touchstart”, “touchmove”, “touchend”, “touchcancel”
control:  “resize”, “scroll”, “zoom”, “focus”, “blur”, “select”, “change”, “submit”, “reset”
no arguments: all of the above + “load”, “unload”, “abort”, “error”, “select”, “change”, “submit”, “reset”, “focus”, “blur”, “resize”, “scroll”, “search”, “devicemotion”, “deviceorientation”
```

Many thanks to (briangrinstead)[http://www.briangrinstead.com/blog/chrome-developer-tools-monitorevents]
