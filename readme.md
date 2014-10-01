Docker Tor Privoxy
==================

Simple single container that sets up a tor proxy via socks and an http proxy to that tor relay.

Run
-----

```bash
$ docker run -p 8118:8118 -i sherzberg/tor-http-proxy
```

Run on daemon
------

```bash
$ docker run -d -p 8118:8118 -i sherzberg/tor-http-proxy
```

Test [local](https://docs.docker.com/installation/)
----------

```bash
$ curl -x http://127.0.0.1:8118  -L http://echoip.com/
```

Test with [boot2docker](https://docs.docker.com/installation/mac/)
--------------------

```bash
$ curl -x http://$(boot2docker ip 2>/dev/null):8118  -L http://echoip.com/
```

You can now connect to the http proxy via port 8118.

License
-------

[See LICENSE](/LICENSE)
