---
layout: page
title: General HTTP FAQ
---

*This page lists Frequently Asked Questions from people who are specifying HTTP extensions like new header fields. See also our [general FAQ](/docs/faq/).*


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Creating New HTTP Headers](#creating-new-http-headers)
  - [What's appropriate to put into a HTTP header?](#whats-appropriate-to-put-into-a-http-header)
  - [How do I specify a new header?](#how-do-i-specify-a-new-header)
  - [What should I name my header?](#what-should-i-name-my-header)
  - [Can header values be UTF-8? Binary?](#can-header-values-be-utf-8-binary)
  - [Can header values be JSON?](#can-header-values-be-json)
- [Creating New HTTP Methods](#creating-new-http-methods)
- [Creating New HTTP Status Codes](#creating-new-http-status-codes)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


## How do I reference the HTTP specification?

Most specifications can get away with referencing
[RFC7230](http://httpwg.github.io/specs/rfc7230.html), the "core" of HTTP. If
you need to reference a specific method, status code or payload consideration,
you'll also probably need to reference
[RFC7231](http://httpwg.github.io/specs/rfc7231.html).

This includes when you're specifying that you're extending HTTP, using HTTP, or
otherwise talking about HTTP in the abstract; these documents define HTTP
overall, and are backwards-compatible with HTTP/1.0 and forwards-compatible
with HTTP/2 (and beyond). 

There isn't any need to reference the HTTP/2 specification directly, unless
you're doing something specific to it (e.g., a new error code, extension frame
type or the like).

If you talk about conditional requests, range requests, caching or
authentication, you might consider referencing RFCs
[7232](http://httpwg.github.io/specs/rfc7232.html),
[7233](http://httpwg.github.io/specs/rfc7233.html),
[7234](http://httpwg.github.io/specs/rfc7234.html) or
[7235](http://httpwg.github.io/specs/rfc7235.html) (respectively.)

RFC1945, RFC2068 and RFC2616 should not be referenced, unless you specifically need to talk about those documents in particular. 

## How do I create a new HTTP header?

### What's appropriate to put into a HTTP header?

### How do I specify a new header?

### What should I name my header?

### Can header values be UTF-8? Binary?

### Can header values be JSON?

## How do I create a new HTTP method?


## How do I create a new HTTP Status Code?