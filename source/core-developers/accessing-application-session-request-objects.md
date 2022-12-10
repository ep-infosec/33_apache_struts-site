---
layout: default
title: Accessing application, session, request objects
parent:
    title: Core Developers Guide
    url: index.html
---

# Accessing application, session, request objects

**DEPRECATED???**

The framework provides several access helpers to access Session, Application, Request scopes.

## Accessing from Java

All the JEE scope attribute maps can be accessed via `ActionContext`.

**Accessing servlet scopes**

```java
Map attr = (Map) ActionContext.getContext().get("attr");
attr.put("myId", myProp);  // Page scope.

Map application = (Map) ActionContext.getContext().get("application");
application.put("myId", myProp);

Map session = (Map) ActionContext.getContext().get("session");
session.put("myId", myProp);

Map request = (Map) ActionContext.getContext().get("request");
request.put("myId", myProp);
```

> Do not use `ActionContext.getContext()` in the constructor of your Action class. The values may not be set up, and 
> the call may return null for getSession().

We can also access the `HttpServletRequest` and `HttpServletResponse` objects themselves through `ServletActionContext`. 
In general this isn't recommended as it will tie our action to the servlet specification.

**Setting session attribute through session object**

```java
ServletActionContext.getRequest().getSession().put("myId", myProp);
```

Implementing `ServletRequestAware` or `ServletResponseAware`, combined with the `servletConfig` interceptor, 
is an alternative way to access the request and response objects, with the same caveat.

## Accessing from the view (JSP, FreeMarker, etc.)

Request and session attributes are accessed via OGNL using the `#session` and `#request` stack values.
Page attributes are accessed via OGNL using the `#attr` stack value, and Application attributes via
the `#application` stack value.

The `#attr` stack value will search the `javax.servlet.jsp.PageContext` for the specified key. If the `PageContext`
doesn't exist, it will search the request, session, and application scopes, in that order.

**Accessing attributes in the Application, Session, Request, or Page scope from a JSP**

```jsp
<p>Retrieve the attribute (property), with key myId, from the specified scope:</p>

<s:property value="#application.myId" />

<s:property value="#session.myId" />

<s:property value="#request.myId" />

<s:property value="#attr.myId" />

<p>Reminder: #attr is for Page scope attributes first, but will search the remaining scopes, in order, seeking a match.</p>
```
