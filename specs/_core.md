
## Core Specifications

The "core" semantics of the HTTP protocol are defined by:

 * RFC9110: [HTTP Semantics](/specs/rfc9110.html)
 * RFC9111: [HTTP Caching](/specs/rfc9111.html)

Those semantics are expressed "on the wire" in three ways:

 * RFC9112: [HTTP/1.1](/specs/rfc9112.html)
 * RFC9113: [HTTP/2](/specs/rfc9113.html)
 * RFC9114: [HTTP/3](/specs/rfc9114.html)

Later versions of HTTP offer field compression:

 * RFC7541: [HPACK Header Compression for HTTP/2](/specs/rfc7541.html)
 * RFC9204: [QPACK Field Compression for HTTP/3](/specs/rfc9204.html)
 
These RFCs collectively obsolete all preceding RFCs defining HTTP, including **RFC1945**, **RFC2068**, **RFC2616**, **RFC2617**, **RFC7230-RFC7235**, and **RFC7540**.

Also relevant is the Structured Field Values specification, which is used in a growing number of headers and trailers:

 * RFC8941: [Structured Field Values for HTTP](/specs/rfc8941.html)
 
Protocols built "on top" of HTTP should follow Best Current Practice, as documented here:

 * RFC9205: [Building Protocols with HTTP](/specs/rfc9205.html)
