## Local Squid Proxy setup

```shell
docker run -it -p 3128:3128 --rm --name squid --mount type=bind,source="$(pwd)"/squid.conf,target=/etc/squid/squid.conf,readonly ubuntu/squid
```