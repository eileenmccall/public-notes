- an application protocol that sits above the communication protocol
- defined to communicate information between two pieces of software via HTTP messages
- the HTTP client (browser) is always initiating the request to the HTTP server
- Request
	- HTTP Headers
		- additional data sent by the user agent to give more context about the transaction going on between the client and the server
		- Methods
			- `OPTIONS`
			- `GET`
			- `HEAD`
			- `POST`
			- `PUT`
			- `DELETE`
			- `TRACE`
			- `CONNECT`
	- URIs
		- niquely identify something on the network
- Response
	- Status Codes
		- `200` - OK
		- `307` - moved temporarily elsewhere
			- useful when you want to redirect a client to a specific page for a little while
		- `301` - address changed permanently