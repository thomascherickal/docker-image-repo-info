## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:3f7c4b5563ba60f3b074abe8c2e9cbbf69da43827e71c3dfa4305015c6212ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull nats-streaming@sha256:149114687b0065b519f88c63c095eb584399006bddda2a1a382b7817926b7dee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170486c15d0c0c7981566004b76d16800fadc1ccb2952c2b0abf6a7754a078c`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:03:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 11 Nov 2021 02:17:43 GMT
RUN cmd /S /C #(nop) COPY file:5c581e1f4c081c37ef7a8184c97600a8222fb8c3e0a6875c5f32e3adfd831c0a in C:\nats-streaming-server.exe 
# Thu, 11 Nov 2021 02:17:44 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Thu, 11 Nov 2021 02:17:45 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Thu, 11 Nov 2021 02:17:46 GMT
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
	-	`sha256:456531efb4db182d63ccf25709a052360ae0086f26f6375b7f1030b7f82c3e87`  
		Last Modified: Thu, 11 Nov 2021 02:21:15 GMT  
		Size: 7.4 MB (7418689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42caa756a767e617e3ae4e035d45621819a45961efd8f86e62efa4c0682a54d0`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a63bf32b10f526a81d26c3a893d32f567ee712e6b0807751f56982f26e36b92`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e98752edcc9e4d3968495bbd12476cba16a5f56641abc2b6407201a7394dbe`  
		Last Modified: Thu, 11 Nov 2021 02:21:12 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
