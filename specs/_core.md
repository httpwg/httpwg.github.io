
## Core Specifications

The "core" semantics of the HTTP protocol are defined by this specification:

 * RFC7231: [HTTP Semantics and Content](/specs/rfc7231.html)

Those semantics are expressed "on the wire" in two different ways:

 * RFC7230: [HTTP/1.1](/specs/rfc7230.html)
 * RFC7540: [HTTP/2](/specs/rfc7540.html)
 * RFC8740: [HTTP/2 with TLS 1.3](/specs/rfc8740.html)

HTTP/2 also uses:

 * RFC7541: [HPACK Header Compression for HTTP/2](/specs/rfc7541.html)

These HTTP functions are optional to implement, but widely used: 
 
 * RFC7232: [HTTP Conditional Requests](/specs/rfc7232.html)
 * RFC7233: [HTTP Range Requests](/specs/rfc7233.html) 
 * RFC7234: [HTTP Caching](/specs/rfc7234.html) 
 * RFC7235: [HTTP Authentication](/specs/rfc7235.html) 
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068**, **RFC2616** and **RFC2617**.

*The core specifications are currently [under revision](https://github.com/httpwg/http-core). If you find issues, please bring them up there!*
