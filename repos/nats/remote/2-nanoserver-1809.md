## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:ce15892fb6be1418971b41da374034da781b7b2344f8cff60a30f8ea0857da13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats@sha256:608cafe97a05f7660f42c078b4bd55ca7632b8e83cad837b2a486deef0d5b02e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107574310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4291bd396e4ecfe7b107395bd83c9427c38d1a4e1c0190feae27b122b16c5f2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 26 Jan 2022 01:18:37 GMT
RUN cmd /S /C #(nop) COPY file:932b1d3725f3eecbc99364f5cd8482f6ade6cced0b1f25a87a9462657422ba86 in C:\nats-server.exe 
# Wed, 26 Jan 2022 01:18:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 26 Jan 2022 01:18:40 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:18:41 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 26 Jan 2022 01:18:42 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839106402c8255997fa7902a05911618c2ef4baf58763e13c9c1dc9d0e93d1ae`  
		Last Modified: Wed, 26 Jan 2022 01:19:39 GMT  
		Size: 4.5 MB (4521329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6ae71bb10c19cdca35a65d89db3a7f1a414ca68d9797f41c33a6cb98978b58`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953cc2c6726f7a88561c57067e9701806e9ab55aedd0dd673deefc8bebd5e2a`  
		Last Modified: Wed, 26 Jan 2022 01:19:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c55a87ac153eac7a04c6b1aade5d653673819e3e33d68b51c2355163db097a7`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0284a6c1c2b8b0a9fa0d10c58d0d787f26d3f48b9b2b19433b1682dba6e38dd4`  
		Last Modified: Wed, 26 Jan 2022 01:19:33 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
