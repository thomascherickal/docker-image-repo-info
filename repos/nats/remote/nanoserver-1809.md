## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:7a2d98a5b753a5dda286d813cd659bbf643273261ff97eed03f2913bec212d14
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110058590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6053b3b2873727cbc239a8f2f188a3a21e24ac6814663edb2ea8f48c8956eb`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:18:05 GMT
RUN cmd /S /C #(nop) COPY file:e96a31c5ad40a0a5eaef053df0a63256800bd64c5d540b7344e9355732202086 in C:\nats-server.exe 
# Fri, 13 Oct 2023 20:18:06 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:18:06 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:18:07 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:18:08 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a381bb328c79ccc2b650690b72d35af9b45846c25f0b1f912c19a399ba590aa9`  
		Last Modified: Fri, 13 Oct 2023 20:22:11 GMT  
		Size: 5.6 MB (5587595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f74fdcc4d1ae922650148dda0bce32832a5cc7921d9b0eb6c123dbaacfbbe0e`  
		Last Modified: Fri, 13 Oct 2023 20:22:10 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf04dfe6fbcb12d208e1d0b116da1d75cd7a0b526af952bc3ab501e7439c528`  
		Last Modified: Fri, 13 Oct 2023 20:22:10 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca4c5016ea5c75e59acf319fc29379b184a2a6ce6db2ffae53f653b0e304eae`  
		Last Modified: Fri, 13 Oct 2023 20:22:10 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682c1be2b093f6f41729a1216304cb75264ee8620eb2cbd29d52c6e1a84fa7d9`  
		Last Modified: Fri, 13 Oct 2023 20:22:10 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
