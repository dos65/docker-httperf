# docker-httperf
built from https://github.com/rtCamp/httperf

[Httperf home page](http://www.hpl.hp.com/research/linux/httperf/)

[Preparing access log for replay](http://schlinkify.org/post/19743846/how-to-replay-live-traffic-with-httperf)

### Example
```
docker run -v [path-to-acees-log-dir]:/[mount-path] dos65/httperf httperf --server [server] 
          --wlog=n,[mount-path/requests] 
          --num-conns [n]
```
