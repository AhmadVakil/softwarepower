---
title: What is CORS (Cross Origin Resource Sharing)
date: 2020-11-15T18:46:11.000Z
updated: 2020-11-15T18:46:11.000Z
category:
  - Learning
comments: true
---
**What is Cross Origin Resource Sharing**

CORS is a security feature implemented in web browsers that allows web applications to make requests to resources on a different domain than the one hosting the web page. It is designed to prevent unauthorized access to resources on different domains, which can be a security risk.

Before CORS, web applications were limited to accessing resources only from the same domain, which could limit their functionality and reduce their usefulness. CORS provides a way for web applications to safely request resources from a different domain, while preventing unauthorized access to those resources.

How does CORS work?

When a web application makes a request to a different domain, the browser sends a preflight request to the server to check if the server allows cross-origin requests. The preflight request includes information about the request, such as the HTTP method, headers, and content type.

The server responds to the preflight request with the Access-Control-Allow-Origin header, which specifies which domains are allowed to make cross-origin requests. The server can also specify which HTTP methods, headers, and content types are allowed in cross-origin requests.

If the response from the server is successful, the browser sends the actual request to the server, including any data or parameters required for the request.

Why is CORS important for web security?

CORS is an important security feature because it prevents malicious scripts from accessing sensitive information on different domains. Without CORS, an attacker could use a cross-site scripting (XSS) attack to inject malicious code into a web page and then access sensitive information from a different domain.

CORS also prevents cross-site request forgery (CSRF) attacks, which occur when an attacker tricks a user into unknowingly making a request to a different domain. By preventing unauthorized requests to different domains, CORS helps to ensure the security and integrity of web applications.

Conclusion

In conclusion, CORS is a security feature that allows web applications to safely request resources from a different domain, while preventing unauthorized access to those resources. It is an important security feature that helps to ensure the security and integrity of web applications. By implementing CORS, developers can create more functional and secure web applications that can access resources from different domains.

