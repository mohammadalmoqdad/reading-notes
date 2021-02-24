## Why is the Context API useful?
- because it can send to more thatn one component

## Can a component outside of a provider get its context?
- No, it is only egetting access for the components in the same tree.
  

## What are some common use cases for using the Context API?
- to move data from parent to children 




# React Cookies:

- Integrations
universal-cookie - Universal cookies for JavaScript
universal-cookie-express - Hook cookies get/set on Express for server-rendering

- On the server, the cookies props must be set using req.universalCookies or new Cookie(cookieHeader)

- setCookie(name, value, [options]):
  - name (string): cookie name
  -  value (string|object): save the value and stringify the object if needed
  -  options (object): Support all the cookie options from RFC 6265

- There are three main components for the array that being set:
1. SetCookie :Function
2. removeCookie () : function
3. the cookies: the value of them?



- withCookies(ComponentGive access to your cookies anywhere
- Add the following props to your component:
  * cookies: Cookies instance allowing you to get, set and remove cookies.
  * allCookies: All your current cookies in an object.


