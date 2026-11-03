# example terminal output from curl

```
[I] eric@roundtable ~> curl -i -X POST localhost:9001/books -H 'Content-Type: application/json' \
                           -d '{"isbn":"12AA7891", "title":"", "author":"", "price":"-9.90"}'
HTTP/1.1 400
Content-Type: application/json
Content-Length: 179
Date: Mon, 02 Nov 2026 23:54:57 GMT
Connection: close

{"author":"The book author must be defined.","price":"The book price must be greater than zero.","isbn":"The ISBN format must be valid.","title":"The book title must be defined."}⏎
```
