---
layout: page
title: Learn about HTTP
---

## Core Specifications

**The core specifications defining the HTTP protocol are:**

 * **RFC7230** - [HTTP/1.1: Message Syntax and Routing](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7230.html) - overview, *message parsing and connections* 
 * **RFC7231** - [HTTP/1.1: Semantics and Content](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7231.html) - *methods, status codes and headers* 
 
Additionally, the following specifications are optional to implement, but widely used: 
 
 * **RFC7232** - [HTTP/1.1: Conditional Requests](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7232.html) - *e.g., If-Modified-Since*
 * **RFC7233** - [HTTP/1.1: Range Requests](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7233.html) - *getting partial content* 
 * **RFC7234** - [HTTP/1.1: Caching](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7234.html) - *browser and intermediary caches* 
 * **RFC7235** - [HTTP/1.1: Authentication](http://svn.tools.ietf.org/svn/wg/httpbis/specs/rfc7235.html) - *HTTP authentication framework* 
 * **RFC6265** - [HTTP State Management Mechanism](http://tools.ietf.org/html/rfc6265) - *cookies (not a WG product)*
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068** and **RFC2616**.


## HTTP Extension Registries

There are a large number of HTTP extensions, including methods, status codes and headers. It's important to note that they are all "part of" HTTP, as long as they're listed in the appropriate registries:

* [HTTP Method Registry](http://www.iana.org/assignments/http-methods/)
* [HTTP Status Code Registry](http://www.iana.org/assignments/http-status-codes/)
* [Message Header Registry](http://www.iana.org/assignments/message-headers/) - *where protocol is 'http'*

Individual headers have their own registries that regulate permissible values, including:

* [HTTP Authentication Scheme Registry](http://www.iana.org/assignments/http-authschemes/) - *WWW-Authenticate, Proxy-Authenticate and related headers*
* [HTTP Cache Directive Registry](http://www.iana.org/assignments/http-cache-directives/) - *Cache-Control*
* [HTTP Parameters](http://www.iana.org/assignments/http-parameters/) - *Content-codings, transfer-codings, Forwarded, Prefer, and Range-related headers*



## Frequently Asked Questions

We have a number of FAQ listings, split up by the intended audience:

* Developer FAQs
* Operations FAQs
* Specification FAQs
