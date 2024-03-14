# HTTP Request and Response Documentation

## Request Details
### POST /userinfo.php HTTP/1.1
- **Host**: testphp.vulnweb.com
- **Connection**: keep-alive
- **Content-Length**: 24
- **Cache-Control**: max-age=0
- **Upgrade-Insecure-Requests**: 1
- **Origin**: http://testphp.vulnweb.com
- **Content-Type**: application/x-www-form-urlencoded
- **User-Agent**: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36
- **Accept**: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
- **Referer**: http://testphp.vulnweb.com/login.php
- **Accept-Encoding**: gzip, deflate
- **Accept-Language**: en-GB,en-US;q=0.9,en;q=0.8

Body:
uname=user&pass=guwgdugj

markdown
Copy code
## Response Details
### HTTP/1.1 302 Found
- **Server**: nginx/1.19.0
- **Date**: Thu, 14 Mar 2024 19:02:18 GMT
- **Content-Type**: text/html; charset=UTF-8
- **Transfer-Encoding**: chunked
- **Connection**: keep-alive
- **X-Powered-By**: PHP/5.6.40-38+ubuntu20.04.1+deb.sury.org+1
- **Location**: login.php

### Note
- The request is a POST request to `userinfo.php` with the parameters `uname` and `pass`.
- The server responds with a 302 Found status, redirecting to `login.php`.

## Subsequent Request Details
### GET /login.php HTTP/1.1
- **Host**: testphp.vulnweb.com
- **Connection**: keep-alive
- **Cache-Control**: max-age=0
- **Upgrade-Insecure-Requests**: 1
- **User-Agent**: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36
- **Accept**: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
- **Referer**: http://testphp.vulnweb.com/login.php
- **Accept-Encoding**: gzip, deflate
- **Accept-Language**: en-GB,en-US;q=0.9,en;q=0.8

## Subsequent Response Details
### HTTP/1.1 200 OK
- **Server**: nginx/1.19.0
- **Date**: Thu, 14 Mar 2024 19:02:19 GMT
- **Content-Type**: text/html; charset=UTF-8
- **Transfer-Encoding**: chunked
- **Connection**: keep-alive
- **X-Powered-By**: PHP/5.6.40-38+ubuntu20.04.1+deb.sury.org+1
- **Content-Encoding**: gzip

### Note
- The subsequent request is a GET request to `login.php`.
- The server responds with a 200 OK status.
- The response contains HTML code for a login page.
