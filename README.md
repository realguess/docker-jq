jq
==

[jq] v1.4 Docker image based on [BusyBox], just over 6MB in size.

[jq]: http://stedolan.github.io/jq/
[BusyBox]: https://registry.hub.docker.com/_/busybox/


Usage
-----

Test `jq` command:

```
$ docker run --rm --name jq realguess/jq:1.4 \
  sh -c 'echo "{\"foo\":\"bar\"}" | jq .'
{
  "foo": "bar"
}
```

Start an interactive container with jq:

```
$ docker run -it --rm --name jq realguess/jq:1.4
```

This will drop into `/bin/sh`, then `jq` command can be run:

```
# jq
```
