---
layout: default
title: ActionEventListener
parent:
    title: Core Developers Guide
    url: index.html
---

# ActionEventListener

An `ActionEventListener` can be used to add some logic when action's instance is created or when exception occurred 
during processing the action.

## Configuration

Right now there can be only one instance of `ActionEventListener` for the whole Struts2 application. You can configure 
it via `struts.xml` by adding bean definition:

```xml
<bean type="com.opensymphony.xwork2.ActionEventListener" class="com.demo.MyActionEventListener"/>
```

## Examples

```java
public class MyActionEventListener implements ActionEventListener {

    public Object prepare(Object action, ValueStack stack) {
        if (action instanceof MyBaseAction) {
            ((MyBaseAction)action).setUserService(stack.findValue("userService"));
        }
    }
    
    public String handleException(Throwable t, ValueStack stack) {
        if (t instanceof MyBusinessException) {
            return stack.findString("defaultBusinesResult");
        }
        return null;
    }
}
```
