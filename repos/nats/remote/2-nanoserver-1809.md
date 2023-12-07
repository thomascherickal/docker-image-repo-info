## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:7e5a1765845a818e657063bc693b2890b02f7860c7355f18618ecc568d6632a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5122; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:656bc68ea443cc235c1106da978257bff6eac8de57b8d87757e6938e9c5bb133
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110104278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e58b567a0c17570ab3d44bd3babe7fca1362f86e38589280c8493394e8e696a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 07 Dec 2023 01:19:09 GMT
RUN cmd /S /C #(nop) COPY file:fc393f320d6ee1aed79e267d10a974b4a909e644d8da91a00b7860f174eacb86 in C:\nats-server.exe 
# Thu, 07 Dec 2023 01:19:10 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:19:11 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 07 Dec 2023 01:19:12 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c3e435696e60abcc593caf5454ef5f07e7ef9695bdfddda9afcd40f060f268`  
		Last Modified: Thu, 07 Dec 2023 01:20:23 GMT  
		Size: 5.6 MB (5600432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e61738ceb98866ba2b4958fcc8b02792a5018cd31ce5ca54acc69e81c0d087`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414d4df9572dfadca1f4bb4237a14c4a08537d4a91f95ec0de7b3c00d32cf013`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8da11653a053c1d821381171f34e78a8259e13f23736d16d5ade220e56f06`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548a0bcd6b9c5bc2c3aa3a4584ff6213adc2d813ddf0fcf7e2f5c0bcfba53720`  
		Last Modified: Thu, 07 Dec 2023 01:20:21 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
