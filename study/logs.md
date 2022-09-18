# Logs Formats

#### NCSA Common log format
Is a standardized format to webservers logs.
```
host ident authuser date request status bytes
```
```
127.0.0.1 user-identifier frank [10/Oct/2000:13:55:36 -0700] "GET /apache_pb.gif HTTP/1.0" 200 2326
```

A dash (-) in a field indicates missing data.

- 127.0.0.1 is the IP address of the client (remote host) which made the request to the server.
- user-identifier is the RFC 1413 identity of the client. Usually "-".
- frank is the userid of the person requesting the document. Usually "-" unless .htaccess has requested authentication.
- [10/Oct/2000:13:55:36 -0700] is the date, time, and time zone that the request was received, by default in strftime format %d/%b/%Y:%H:%M:%S %z.
- "GET /apache_pb.gif HTTP/1.0" is the request line from the client. The method GET, /apache_pb.gif the resource requested, and HTTP/1.0 the HTTP protocol.
- 200 is the HTTP status code returned to the client. 2xx is a successful response, 3xx a redirection, 4xx a client error, and 5xx a server error.
- 2326 is the size of the object returned to the client, measured in bytes.
