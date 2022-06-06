
## Extension Registries

There are a large number of HTTP extensions, including methods, status codes and headers. It's important to note that they are all "part of" HTTP, as long as they're listed in the appropriate registries:

* [HTTP Method Registry](http://www.iana.org/assignments/http-methods/) - _[more info](/specs/rfc9110.html#method.registry)_
* [HTTP Status Code Registry](http://www.iana.org/assignments/http-status-codes/) - _[more info](/specs/rfc9110.html#status.code.registry)_
* [Message Header Registry](http://www.iana.org/assignments/message-headers/) *where protocol is 'http'* - _[more info](/specs/rfc9110.html#fields.registry)_
* [HTTP/2 Parameters](http://www.iana.org/assignments/http2-parameters/http2-parameters.xhtml) - *Frame types, settings, error codes*

Individual headers have their own registries that regulate permissible values, including:

* [HTTP Authentication Scheme Registry](http://www.iana.org/assignments/http-authschemes/) - _[more info](/specs/rfc9110.html#auth.scheme.registry)_
* [HTTP Cache Directive Registry](http://www.iana.org/assignments/http-cache-directives/) - _[more info](/specs/rfc9111.html#cache.directive.registry)_
* [HTTP Parameters](http://www.iana.org/assignments/http-parameters/) - *Content-codings, transfer-codings, Forwarded, Prefer, and Range-related headers*
