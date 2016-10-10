# PicoLisp Docker Image

This Docker Image compiles a [picoLisp 64](http://picolisp.com/wiki/?home) system from the source
distribution.

to use it, pull the Dockerfile image:

```
docker pull turbopape/docker-picolisp
```

Then run it using a volume to persist your work:

```
alias pil='docker run -v ~/work:/usr/local/work -it docker-picolisp'
pil
```
I will try to stay on par with picoLisp releases.

This Dockerfile was inspired
by
[iprog4u/docker-tinycore-picolisp](https://github.com/iprog4u/docker-tinycore-picolisp),
but uses source distributions, so might be more up-to-date with the
upstream releases. One possible inconvenience with this is that the
size of this image might be bigger, as it contains gcc, java and the
glibc.

# License

This is released under the terms of the [MIT License.](./LICENSE)
