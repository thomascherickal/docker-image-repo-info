## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:4a05c1492bc9c9c98fcf83005a908b7bc77548af38ec3a509f134077c7c50937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:a7f29493dab913be41f0cf6051779c0d546db0da3b7fb8167638f422e355d15e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110210052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6750b316cf0dd053c2fee747f6e634f92b9eaa112626290079d4cf1e54a74502`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 20 Nov 2021 00:17:57 GMT
RUN cmd /S /C #(nop) COPY file:bb30895f60b97f75adc45bbc64dd23d70df079c19ad26c4f8d07ce1c88e77c96 in C:\nats-streaming-server.exe 
# Sat, 20 Nov 2021 00:17:58 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Sat, 20 Nov 2021 00:17:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Sat, 20 Nov 2021 00:18:00 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1d3f90d67d7551be12e9caf53f786235234151f513c0aadc754e5f033e183641`  
		Last Modified: Wed, 10 Nov 2021 17:06:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fff8078017e96d5452cd0e323a3b37608d78ba4cafe2372980024ca55f0c206`  
		Last Modified: Sat, 20 Nov 2021 00:21:34 GMT  
		Size: 7.4 MB (7422491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2145022064c695ab600037837d502e536f4f7a4e6450759fbdf9ebd45db54f2c`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf1a2b0c8b67cf32eb3c79e5231671c4c630febe3335f197932a5ee788d26f1`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3816622dce5ac632e33bd266c424f4c291d5b69012c3dbe669262447bc12bc`  
		Last Modified: Sat, 20 Nov 2021 00:21:32 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
