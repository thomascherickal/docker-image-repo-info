## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:368b565836a5cb8a1a9e3ba4060be27137b1fe18c0bf11d10d431ef2d3e5b2fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:df516879fec4e8ccc8ae6ac6aea53c2e6a0a3523d7b41c302a7985a0b7995d3a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110193630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309044877ff486147a6a46155ebe4d992cdde2199438cb80818c37fcd4b4b2fc`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Nov 2021 20:06:58 GMT
RUN cmd /S /C #(nop) COPY file:b51e73a1c237a3ceabbedb6df922d408b584eda17f8a45520b9f3340b551e973 in C:\nats-streaming-server.exe 
# Wed, 10 Nov 2021 20:06:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Nov 2021 20:07:00 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 10 Nov 2021 20:07:01 GMT
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
	-	`sha256:52c13b5e5b16544336e0a77bb2f639c9c7ba2af451247080a8fe54a8fbf04edd`  
		Last Modified: Wed, 10 Nov 2021 20:10:26 GMT  
		Size: 7.4 MB (7406130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f0d6bdec2654253b07eea30be908fb3ca7367a25f1a62c92d3646573a041d3`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a28a82fbcaa742a149084899f63e389bafa95fb6f9da5f47459937b71aade0`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7614d3d321a982272f72712b82654dcf46c7eaecd5c50e8917c70af3efd3cd73`  
		Last Modified: Wed, 10 Nov 2021 20:10:24 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
