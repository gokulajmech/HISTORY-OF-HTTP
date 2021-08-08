
HTTP (Hyper Text Transfer Protocol)


DEVELOPERS
 Tim Berners-Lee and his team (1989-1991)
 
 
EVALUTION
	Initially calling it the Mesh, it was later renamed to World Wide Web during its implementation in 1990. 
Built over the existing TCP and IP protocols.


VERSIONS WITH FEATURES

	HTTP/0.9, HTTP/1.0, HTTP/1.1, and HTTP/2.0
  
1.HTTP/0.9 – The one-line protocol
The initial version of HTTP had no version number; it has been later called 0.9 to differentiate it from the later versions. 
HTTP/0.9 is extremely simple: requests consist of a single line 
There were no HTTP headers, meaning that only HTML files could be transmitted, but no other type of documents. There were no status or error codes, in case of a problem, a specific HTML file was sent back with the description of the problem contained in it, for human consumption.

	2.HTTP/1.0 – Building extensibility
HTTP/0.9 was very limited and both browsers and servers quickly extended it to be more versatile:
•	Versioning information is now sent within each request 
•	A status code line is also sent at the beginning of the response, 
•	The notion of HTTP headers has been introduced, both for the requests and the responses.
•	plain HTML files has been added .

3.HTTP/1.1 – The standardized protocol
HTTP/1.1 clarified ambiguities and introduced numerous improvements:
•	A connection can be reused, saving the time to reopen it numerous times to display the resources embedded into the single original document retrieved.
•	Pipelining has been added, allowing to send a second request before the answer for the first one is fully transmitted, lowering the latency of the communication.
•	Chunked responses are now also supported.
•	Additional cache control mechanisms have been introduced.
•	Content negotiation, including language, encoding, or type, has been introduced, and allows a client and a server to agree on the most adequate content to exchange.
•	The ability to host different domains at the same IP address now allows server colocation.

4.HTTP/2 – A protocol for greater performance
•	It is a binary protocol rather than text. It can no longer be read and created manually. Despite this hurdle, improved optimization techniques can now be implemented.
•	It is a multiplexed protocol. Parallel requests can be handled over the same connection, removing the order and blocking constraints of the HTTP/1.x protocol.
•	It compresses headers. As these are often similar among a set of requests, this removes duplication and overhead of data transmitted.
•	It allows a server to populate data in a client cache, in advance of it being required, through a mechanism called the server push.



