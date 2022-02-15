# go-url-shorten

A URL shortning api using
- Redis as DB
- GoFiber for server
- Docker

---

### Routes
`GET localhost:9090/:short` redirects to the correct url as stored in DB
`POST localhost:9090/api/v1/ body:{url: "The url to redirect", "short":"custom short string(optional)}` gives the shortened url and tells the rate limiting quota left for your ip
