#### Alpine Privoxy

## Usage

example：

``` bash
docker run -d -p 8118:8118 -v ./config:/etc/privoxy/config xiaomingyang/privoxy
```

config file:

```
listen-address  0.0.0.0:8118
forward-socks5 / 10.1.1.1:1080 .
```

