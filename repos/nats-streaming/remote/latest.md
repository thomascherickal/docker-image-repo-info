## `nats-streaming:latest`

```console
$ docker pull nats-streaming@sha256:46214f4467deabc181784961b7819d2d094c1b3c1b9ac2507548d054a5c80200
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2458; amd64

### `nats-streaming:latest` - linux; amd64

```console
$ docker pull nats-streaming@sha256:c690399d0d8b57683c4ba6e7aa22e45b1357d52ab101cf7360d7d1064d2d9b25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7043385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:744a834f04a473e985a261e8d8c3fa1d0c00e6a771922395d0ebae6d10c38874`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 19:20:40 GMT
COPY file:b4e3c516d371abb6bcaccca9ba46a1254d1d448565b62e90258b2e38be81e5c3 in /nats-streaming-server 
# Mon, 07 Feb 2022 19:20:40 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:20:40 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 19:20:41 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b6be2016859a5cd8a50b0bd6a05bed6aad13d9debb0bbe0477d969b48d2cd53e`  
		Last Modified: Mon, 07 Feb 2022 19:21:21 GMT  
		Size: 7.0 MB (7043385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:d7009db6cb0db2d097f43ae6122842b3da194df3619e177b4a161df3439a52d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6560060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905e423db0a198c0195925fa6e9375729dcc36f759428cf24b760bf829dbab73`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:50:00 GMT
COPY file:2e99e463744b121a0337cd4461893f5f1868c7757b4a39d1cafecfa830bf9914 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:50:01 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:50:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:50:02 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:198dd57862ff84f4e356d372ae9d9ac254682f54527243974ca5fddf5433eccc`  
		Last Modified: Mon, 07 Feb 2022 18:51:58 GMT  
		Size: 6.6 MB (6560060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:db9679a68ed5cdcea359189ab601b937b2f31c61e18b42aa589a27ed23d7c540
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6550494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:697577adc9268ac41f874a3ef8a949f1bb0f8aa6880b970294ca68ccf5109554`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:58:13 GMT
COPY file:8621f665c3af5dc3ff9730b201529ad96d3a8073ba717219f1fcc6c96730866b in /nats-streaming-server 
# Mon, 07 Feb 2022 18:58:14 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:58:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:58:15 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fa2ff8948be8f6d7e9a084e27f657473b04c0d4b4ac73c7de0e7a62cc67c564f`  
		Last Modified: Mon, 07 Feb 2022 19:00:10 GMT  
		Size: 6.6 MB (6550494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:df26eb0c8179a0eb083277efdc883331715079602ce7654216ebbf39e54a0409
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6473285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72a4ca115226e021e3d0184efffc8d259064859ae98f6db050b5fe87f303e493`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 07 Feb 2022 18:40:23 GMT
COPY file:9911efb61f2f3a79edcdc4545b0b68b1e5584683392e6b8b77f325366fc6eb27 in /nats-streaming-server 
# Mon, 07 Feb 2022 18:40:23 GMT
EXPOSE 4222 8222
# Mon, 07 Feb 2022 18:40:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 07 Feb 2022 18:40:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:fd7fc3f67794629fa56b5709d0394172bed012d6d0f92b1b9c3e789ce4ae8fe9`  
		Last Modified: Mon, 07 Feb 2022 18:41:24 GMT  
		Size: 6.5 MB (6473285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:latest` - windows version 10.0.17763.2458; amd64

```console
$ docker pull nats-streaming@sha256:cffc8ed7be354dfe55472592b9f13e5688826b06953e729d04ea878314a1f8b9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110203881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac225c5e445b78e836f8bca80bdf016e81b69e80553400917c3e58ba551f9a0`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 26 Jan 2022 01:18:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 07 Feb 2022 19:19:39 GMT
RUN cmd /S /C #(nop) COPY file:960f1d98f42f331ed968d42bdc16b58e37407aa1f36a1518de144d635030e72e in C:\nats-streaming-server.exe 
# Mon, 07 Feb 2022 19:19:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 07 Feb 2022 19:19:42 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 07 Feb 2022 19:19:43 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5cb841e15906c5eda43ff713132f917ee3c8f180a706900af652f1e93eeb1790`  
		Last Modified: Wed, 26 Jan 2022 01:19:36 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1689a334d519e2947190597c4c844dc80245b627c8713aea637288f8ad1ea96a`  
		Last Modified: Mon, 07 Feb 2022 19:20:34 GMT  
		Size: 7.2 MB (7152693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a85d66582e7438c7db41e68288a84bc669410c0aec9ed554e69391cd0cdcefa`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd35dd9d78a9ca4e13f2e4a9a4bed7e927a15709a4d436601b9a5dbc1574669b`  
		Last Modified: Mon, 07 Feb 2022 19:20:31 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ffee7517a90df6b9d1ae9232e626ed3dedcd9e8f467981ec21e419bd5338e5`  
		Last Modified: Mon, 07 Feb 2022 19:20:32 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
