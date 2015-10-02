
## Core Specifications

The "core" of the HTTP protocol is defined by two specifications:

 * RFC7230: [HTTP/1.1 Message Syntax and Routing](/specs/rfc7230.html)
 * RFC7231: [HTTP/1.1 Semantics and Content](/specs/rfc7231.html)

HTTP/2 is an updated way to use HTTP "on the wire". and is an alternative to _parts_ of RFC7230. See the <a href="https://http2.github.io/">HTTP/2 Home</a> for more.

 * RFC7540: [HTTP/2](/specs/rfc7540.html)
 * RFC7541: [HPACK Header Compression for HTTP/2](/specs/rfc7541.html)
 
Additionally, the following are optional to implement, but widely used: 
 
 * RFC7232: [HTTP/1.1 Conditional Requests](/specs/rfc7232.html)
 * RFC7233: [HTTP/1.1 Range Requests](/specs/rfc7233.html) 
 * RFC7234: [HTTP/1.1 Caching](/specs/rfc7234.html) 
 * RFC7235: [HTTP/1.1 Authentication](/specs/rfc7235.html) 
 * RFC7616: [HTTP Digest Access Authentication](/specs/rfc7616.html)
 * RFC7617: [HTTP Basic Authentication](/specs/rfc7617.html)
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068**, **RFC2616** and **RFC2617**.

*If you find problems with the HTTP/1.1 specifications, you can log an issue in [this repo](https://github.com/httpwg/http11bis/issues).*