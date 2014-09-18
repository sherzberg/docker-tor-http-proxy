Docker Tor Privoxy
==================

Simple single container that sets up a tor proxy via socks and an http proxy to that tor relay.

Usage
-----

```bash
$ docker run -p 8118:8118 -i sherzberg/tor-http-proxy
```

You can now connect to the http proxy via port 8118.

License
-------

[See LICENSE](/LICENSE)
