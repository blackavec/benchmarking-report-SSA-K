# Running benchmark
```
ab -n 20 -c 1 -r http://localhost:3000/ 
```

# Hypotheses 

1 - SSR + react is slow without caching mechanism.

**Pre server cache**
```
Requests per second:    1.32 [#/sec] (mean)
```
[Learn more](./ab-benchmark-20req-1cuncurrent-pre-cache.log)

**Post server cache**
```
Requests per second:    203.75 [#/sec] (mean)
```
[Learn more](./ab-benchmark-20req-1cuncurrent-post-cache.log)

**Result**
caching is effective to reduce the page load.
