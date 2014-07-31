---
layout: page
title: Learn about HTTP
---

## Core Specifications

**The core specifications defining the HTTP protocol are:**

 * **RFC7230** - [HTTP/1.1: Message Syntax and Routing](/specs/rfc7230.html) - overview, *message parsing and connections* 
 * **RFC7231** - [HTTP/1.1: Semantics and Content](/specs/rfc7231.html) - *methods, status codes and headers* 
 
Additionally, the following specifications are optional to implement, but widely used: 
 
 * **RFC7232** - [HTTP/1.1: Conditional Requests](/specs/rfc7232.html) - *e.g., If-Modified-Since*
 * **RFC7233** - [HTTP/1.1: Range Requests](/specs/rfc7233.html) - *getting partial content* 
 * **RFC7234** - [HTTP/1.1: Caching](/specs/rfc7234.html) - *browser and intermediary caches* 
 * **RFC7235** - [HTTP/1.1: Authentication](/specs/rfc7235.html) - *HTTP authentication framework* 
 * **RFC6265** - [HTTP State Management Mechanism](/specs/rfc6265.html) - *cookies (not a WG product)*
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068** and **RFC2616**.


## HTTP Extensions

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

* [General HTTP FAQs](faq/) - *try here first*
* [Implementation FAQs](faq_dev/) - *questions about implementing HTTP servers and clients*
* [Specification FAQs](faq_spec/) - *how to read the HTTP specs and write extensions*
