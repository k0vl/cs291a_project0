# k0vl

GitHub Page. This is not my perosnal page. It is only used for CS 291A Assignment.

## Link

[https://k0vl.github.io/](https://k0vl.github.io/)

## CS 291A Questions

* On average, how many requests can ab complete in 10 seconds with various power of two concurrency levels between 1 and 256?

  concurrency 1: 460.0\
  concurrency 2: 1019.5\
  concurrency 4: 2050.0\
  concurrency 8: 4005.0\
  concurrency 16: 6303.5\
  concurrency 32: 10461.0\
  concurrency 64: 13613.5\
  concurrency 128: 14761.5\
  concurrency 256: 13973.0

* Why are there diminishing returns at higher concurrency levels?

  Either the client or the server could have a limit on open or half-open connections. They could stop making or accepting new connections until old connections are closed. It could also simply have ran out cpu, memory, or network resources.

* What’s the performance difference when requesting HTTP and HTTPS?

  HTTPS, 10s: 528.0 = 0.018939s per request\
  HTTP, 10s: 1273.5 = 0.007852s per request\
  diff = 0.011087s per request\
  141% increase over HTTP

* How can github respond so quickly?

  Because it is serving static websites, so there is minimal processing on the server end. Moreover, it probably uses CDN, loadbalancer, or some forms of cache to accelerate the loading.

* What is your site’s “Time to Interactive” according to PageSpeed Insights?

  1.7 s


