# timeout-checker
A simple wait and response api to test retry& timeout. Yep! Everyone loves retry and timeout test 🤠

Install via brew 
```
$ brew tap applegreengrape/timeout-checker https://github.com/applegreengrape/timeout-checker
$ brew install timeout-checker
```
server side:
```
$ checker-api -wait 5 -port 8081
2021/11/19 16:37:06 recieved
2021/11/19 16:37:11 returned
2021/11/19 16:37:14 recieved
2021/11/19 16:37:19 returned
```

client side:
```
$ curl http://localhost:8081/healthcheck
{"status":"up"}

$ curl http://localhost:8081/healthcheck
{"status":"up"}
```
