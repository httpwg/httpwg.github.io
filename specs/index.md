---
layout: page
title: HTTP Documentation
---

## Core Specifications

The "core" of the HTTP protocol is defined by two specifications:

 * **RFC7230** - [HTTP/1.1: Message Syntax and Routing](/specs/rfc7230.html) - overview, *message parsing and connections* 
 * **RFC7231** - [HTTP/1.1: Semantics and Content](/specs/rfc7231.html) - *methods, status codes and headers* 
 
Additionally, the following specifications are optional to implement, but widely used: 
 
 * **RFC7232** - [HTTP/1.1: Conditional Requests](/specs/rfc7232.html) - *e.g., If-Modified-Since*
 * **RFC7233** - [HTTP/1.1: Range Requests](/specs/rfc7233.html) - *getting partial content* 
 * **RFC7234** - [HTTP/1.1: Caching](/specs/rfc7234.html) - *browser and intermediary caches* 
 * **RFC7235** - [HTTP/1.1: Authentication](/specs/rfc7235.html) - *HTTP authentication framework* 
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068** and **RFC2616**.

*If you find problems with the HTTP/1.1 specifications, you can report them as [errata](http://www.rfc-editor.org/errata.php) on the appropriate specification, or log an issue in [this repo](https://github.com/httpwg/http11bis/issues).*

## Extension Registries

There are a large number of HTTP extensions, including methods, status codes and headers. It's important to note that they are all "part of" HTTP, as long as they're listed in the appropriate registries:

* [HTTP Method Registry](http://www.iana.org/assignments/http-methods/) ([more info](/specs/rfc7231.html#method.registry))
* [HTTP Status Code Registry](http://www.iana.org/assignments/http-status-codes/) ([more info](/specs/rfc7231.html#status.code.registry))
* [Message Header Registry](http://www.iana.org/assignments/message-headers/) - *where protocol is 'http'* ([more info](http://tools.ietf.org/html/rfc3864))

Individual headers have their own registries that regulate permissible values, including:

* [HTTP Authentication Scheme Registry](http://www.iana.org/assignments/http-authschemes/) - *WWW-Authenticate, Proxy-Authenticate and related headers* ([more info](/specs/rfc7235.html#authentication.scheme.registry))
* [HTTP Cache Directive Registry](http://www.iana.org/assignments/http-cache-directives/) - *Cache-Control* ([more info](/specs/rfc7234.html#cache.directive.registry))
* [HTTP Parameters](http://www.iana.org/assignments/http-parameters/) - *Content-codings, transfer-codings, Forwarded, Prefer, and Range-related headers*

## Extension Specifications

This is a **partial** list of HTTP-relevant specifications, here for convenience. For the complete
list, see the relevant extension registry listed above.

### Status Codes

* **RFC7538** - [HTTP Status Code 308 (Permanent Redirect)](/specs/rfc7538.html)
 
 
### Header Fields

* **RFC6265** - [HTTP State Management Mechanism](/specs/rfc6265.html) - *cookies*
