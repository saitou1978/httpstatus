## cgi-bin/index.cgi
### Demo
http://viruupaaksa.com/

### Usage

```
$ curl -I http://<your-server-address>/
HTTP/1.1 200 OK
Date: Sun, 05 Apr 2015 04:54:16 GMT
Server: Apache
Vary: Accept-Encoding
Content-Type: text/html; charset=utf-8
```

```
$ curl -I http://<your-server-address>/index.cgi?code=404
HTTP/1.1 404 Not Found
Date: Sun, 05 Apr 2015 04:54:33 GMT
Server: Apache
Vary: Accept-Encoding
Content-Type: text/html; charset=utf-8
```

```
$ curl -i 'http://<your-server-address>/index.cgi?word=Hello,%20World!&code=404'
HTTP/1.1 404 Not Found
Date: Sun, 05 Apr 2015 06:39:54 GMT
Server: Apache
Vary: Accept-Encoding
Content-Type: text/html; charset=utf-8
Transfer-Encoding: chunked


<html>
<head>
    <title><your-server-address></title>
</head>
<body>
    <h1>Hello, World!</h1>
    <div>404 Not Found</div>
</body>
</html>
```
# httpstatus
