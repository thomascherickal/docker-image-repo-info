## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:3b9cdf089fcb084384e991531227a29c230482b4e682fa252a4340149647be7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull hello-world@sha256:ba3301a6b62903dd9b8cf562548c778ca787f3fe15841b7e2291e91919694ce4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.3 MB (101282171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ede58bc7b806cde5c26148f6de1b02b81c20a87660ec08d91373660feca9a1`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sat, 31 Oct 2020 05:10:43 GMT
RUN Apply image 1809-amd64
# Wed, 11 Nov 2020 13:42:49 GMT
RUN cmd /S /C #(nop) COPY file:0afaffc2fa64462107b7178b2ae7d20404ff12f637eabe3a8046192b9d9a0338 in C: 
# Wed, 11 Nov 2020 13:42:49 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:f1b217fe8837d4d85cb8228a52344d3504d7aa51ba30167a20a6a4cb80cdcaa0`  
		Size: 101.3 MB (101279682 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:96ea7fed2edd8e5e5856d37604695857a79d3fe3b8ca8aaf479b10f5093f9679`  
		Last Modified: Wed, 11 Nov 2020 13:43:00 GMT  
		Size: 1.6 KB (1604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abf9c5f6128d88fc4ae04ecdf91089d14da6ccee40db91354cdf49dd5b7ba69`  
		Last Modified: Wed, 11 Nov 2020 13:43:00 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
