# Type of XSS :

- **Reflected XSS** : occurs when user input is **immediately** returned by a web app in an error message, search result, or any other response that includes some or all of the input provided by the user as part pf the request.
- **Stored XSS** : occurs when user input is stored on the target server (such as in a database, in a message forum, visitor log, comment field, etc).
- **DOM Based XSS** : is an XSS attack wherein the attack payload is executed as a result of modifying the DOM "environment" in the victim's browser used by the original client side script

---------

# Types of Cross-Site Scripting :

- **Client XSS** : occurs when untrusted user supplied data is used to update the DOM with an unsafe Javascript call.
- **Server XSS** : occurs when untrusted user supplied data is included in an HTTP response generated by the Server.

| XSS       | Server               | Client               |
| --------- | -------------------- | -------------------- |
| Stored    | Stored Server XSS    | Stored Client XSS    |
| Reflected | Reflected Server XSS | Reflected Client XSS |

- DOM-Based XSS is subset of Client XSS (where the data source is from the client only).

---------

# Defenses :

##### Recommended Server XSS Defenses :

Server XSS is caused by including untrusted data in an HTML response. The easiest and strongest defense against server XSS :

- Context-sensitive server side output encoding.

##### Recommended Client XSS Defenses :

Client XSS is caused when untrusted data is used to update the DOM with an unsafe JS call.

- Using safe JavaScript APIs