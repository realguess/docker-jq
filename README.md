jq
==

[jq] v1.4 Docker image based on [BusyBox], just over 6MB in size.

[jq]: http://stedolan.github.io/jq/
[BusyBox]: https://registry.hub.docker.com/_/busybox/


Usage
-----

Test `jq` command:

```
$ echo "{\"foo\":\"bar\"} | docker run --rm -i realguess/jq .
{
  "foo": "bar"
}
```

Start an interactive container with jq:

```
$ docker run -it --rm --entrypoint sh realguess/jq:1.4
```

This will drop into `/bin/sh`, then `jq` command can be run:

```
# jq
```
