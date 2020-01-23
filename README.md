## Rate Limit

```bash
open http://localhost/s1/wf
```

## Tests

```bash
brew install wrk
wrk -t2 -d5s http://localhost/s1/wf
wrk -t1 -d5s http://localhost/s1/wf
wrk -t1 -d5s https://google.com

wrk -t20 -c20 -d5s http://localhost/s1/wf
wrk -d5s http://localhost/s1/wf
```