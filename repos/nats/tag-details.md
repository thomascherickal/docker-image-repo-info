<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `nats`

-	[`nats:2`](#nats2)
-	[`nats:2-alpine`](#nats2-alpine)
-	[`nats:2-alpine3.18`](#nats2-alpine318)
-	[`nats:2-linux`](#nats2-linux)
-	[`nats:2-nanoserver`](#nats2-nanoserver)
-	[`nats:2-nanoserver-1809`](#nats2-nanoserver-1809)
-	[`nats:2-scratch`](#nats2-scratch)
-	[`nats:2-windowsservercore`](#nats2-windowsservercore)
-	[`nats:2-windowsservercore-1809`](#nats2-windowsservercore-1809)
-	[`nats:2.10`](#nats210)
-	[`nats:2.10-alpine`](#nats210-alpine)
-	[`nats:2.10-alpine3.18`](#nats210-alpine318)
-	[`nats:2.10-linux`](#nats210-linux)
-	[`nats:2.10-nanoserver`](#nats210-nanoserver)
-	[`nats:2.10-nanoserver-1809`](#nats210-nanoserver-1809)
-	[`nats:2.10-scratch`](#nats210-scratch)
-	[`nats:2.10-windowsservercore`](#nats210-windowsservercore)
-	[`nats:2.10-windowsservercore-1809`](#nats210-windowsservercore-1809)
-	[`nats:2.10.3`](#nats2103)
-	[`nats:2.10.3-alpine`](#nats2103-alpine)
-	[`nats:2.10.3-alpine3.18`](#nats2103-alpine318)
-	[`nats:2.10.3-linux`](#nats2103-linux)
-	[`nats:2.10.3-nanoserver`](#nats2103-nanoserver)
-	[`nats:2.10.3-nanoserver-1809`](#nats2103-nanoserver-1809)
-	[`nats:2.10.3-scratch`](#nats2103-scratch)
-	[`nats:2.10.3-windowsservercore`](#nats2103-windowsservercore)
-	[`nats:2.10.3-windowsservercore-1809`](#nats2103-windowsservercore-1809)
-	[`nats:2.9`](#nats29)
-	[`nats:2.9-alpine`](#nats29-alpine)
-	[`nats:2.9-alpine3.18`](#nats29-alpine318)
-	[`nats:2.9-linux`](#nats29-linux)
-	[`nats:2.9-nanoserver`](#nats29-nanoserver)
-	[`nats:2.9-nanoserver-1809`](#nats29-nanoserver-1809)
-	[`nats:2.9-scratch`](#nats29-scratch)
-	[`nats:2.9-windowsservercore`](#nats29-windowsservercore)
-	[`nats:2.9-windowsservercore-1809`](#nats29-windowsservercore-1809)
-	[`nats:2.9.23`](#nats2923)
-	[`nats:2.9.23-alpine`](#nats2923-alpine)
-	[`nats:2.9.23-alpine3.18`](#nats2923-alpine318)
-	[`nats:2.9.23-linux`](#nats2923-linux)
-	[`nats:2.9.23-nanoserver`](#nats2923-nanoserver)
-	[`nats:2.9.23-nanoserver-1809`](#nats2923-nanoserver-1809)
-	[`nats:2.9.23-scratch`](#nats2923-scratch)
-	[`nats:2.9.23-windowsservercore`](#nats2923-windowsservercore)
-	[`nats:2.9.23-windowsservercore-1809`](#nats2923-windowsservercore-1809)
-	[`nats:alpine`](#natsalpine)
-	[`nats:alpine3.18`](#natsalpine318)
-	[`nats:latest`](#natslatest)
-	[`nats:linux`](#natslinux)
-	[`nats:nanoserver`](#natsnanoserver)
-	[`nats:nanoserver-1809`](#natsnanoserver-1809)
-	[`nats:scratch`](#natsscratch)
-	[`nats:windowsservercore`](#natswindowsservercore)
-	[`nats:windowsservercore-1809`](#natswindowsservercore-1809)

## `nats:2`

```console
$ docker pull nats@sha256:a7896fa3caaffacae323f1777007005298abd0524c6aced0af5c48a39e49062f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4974; amd64

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

## `nats:2-alpine`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4974; amd64

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

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4974; amd64

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

## `nats:2-scratch`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10`

```console
$ docker pull nats@sha256:b61267af0ee231f1aa60394566f555bd0506f3a3172773aa50f3f772f4f5d326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10-alpine`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine3.18`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-linux`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-linux` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-nanoserver` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10-nanoserver-1809`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-nanoserver-1809` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10-scratch`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore-1809`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3`

```console
$ docker pull nats@sha256:b61267af0ee231f1aa60394566f555bd0506f3a3172773aa50f3f772f4f5d326
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.3` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10.3-alpine`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3-alpine3.18`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.3-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3-linux`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3-nanoserver`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.3-nanoserver` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10.3-nanoserver-1809`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.3-nanoserver-1809` - windows version 10.0.17763.4974; amd64

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

## `nats:2.10.3-scratch`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3-windowsservercore`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.3-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.3-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:664aad0be228e0f38246ff04e7dcb84487b33dc8f3cc13e5ff09c77de0fc3245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2493aea2c3d9f0cbd5842f9e7cf0ae1cca872dcab55b986634737fc0bea98c67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9273216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7989a8298522649a1adb3ca614130cb34f8bf861930fdaae0cf9cf7fe777a8ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:12 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:14 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86325e476145954afe4454d6a34d1a8ee010d39db18e02ccc18f3173c1f76c5`  
		Last Modified: Fri, 13 Oct 2023 20:21:48 GMT  
		Size: 5.9 MB (5870249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e197bedf457b6e20573397488cb470629dbb34103b46f2e8afc0fdf0a04aac`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fee3723b24b5f8fe02d83f43f4c5e58a7c7d7e9ad295e1090b5c1121de96ad`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:043a42240b54eff4efa7d2e58782a319fbfb8ccfb9014a94ad57ee293f4710bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8753049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992beb8b085db72a7b6711b774ba559b93c96a4dc4cb0e20eba05a1ff404c9b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:28 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:49:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a705d77fc05da36aa7a1f8f5edb42ad0a278354d7818a46aa366c08c05a9a6`  
		Last Modified: Fri, 13 Oct 2023 20:50:26 GMT  
		Size: 5.6 MB (5606755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be03a937e4af6607f76e748896ccb9bef922488c0ef296120d5170af713977`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516a13f6149cde95784c4dda86214c8e6f629d8b54e67daada10eaedbf16495`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:eb82136d1b0694facbb0e165c28bc2b2b3e43a7207c374c40f14adcdd9fe6a5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8498721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed722d660c639a4623ea7c313732b1214276b7a49aba5feb382c777e952fb3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:33 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:57:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c49c2f4ef415f61afc8f8767700f415271abad05a93c86409223f1ffb582208`  
		Last Modified: Fri, 13 Oct 2023 20:58:52 GMT  
		Size: 5.6 MB (5597814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18deea0b99d1bfaa5737ee833ffc88a535378e7a3386666be65db239e9a797a8`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3671dc5372433df623beb235abc94e688e644e85f86d0347b179526fd165a9c`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:bf7b9a4e1a05493d11d86fc493d67ebf11625e7eff0ee5afd733ae6ccab82556
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8740997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1560dbaf5cdd6a5be38a9524c91d39c8753eb99151610fdfc2fb16b46729d899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:49 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:51 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fe93b371732f5508e482212d76c6956399d79b2ae4994aea9ba1b8fd2e4e9`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 5.4 MB (5408164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bf467ad52a7ee8fe861954ccf4a8a2d09502bbb044dc43820d41608e2711f`  
		Last Modified: Fri, 13 Oct 2023 20:41:28 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc00028abee22a182dd921dc31227b33b33bd7f21227966a71df41bd97cfad08`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:664aad0be228e0f38246ff04e7dcb84487b33dc8f3cc13e5ff09c77de0fc3245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2493aea2c3d9f0cbd5842f9e7cf0ae1cca872dcab55b986634737fc0bea98c67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9273216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7989a8298522649a1adb3ca614130cb34f8bf861930fdaae0cf9cf7fe777a8ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:12 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:14 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86325e476145954afe4454d6a34d1a8ee010d39db18e02ccc18f3173c1f76c5`  
		Last Modified: Fri, 13 Oct 2023 20:21:48 GMT  
		Size: 5.9 MB (5870249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e197bedf457b6e20573397488cb470629dbb34103b46f2e8afc0fdf0a04aac`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fee3723b24b5f8fe02d83f43f4c5e58a7c7d7e9ad295e1090b5c1121de96ad`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:043a42240b54eff4efa7d2e58782a319fbfb8ccfb9014a94ad57ee293f4710bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8753049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992beb8b085db72a7b6711b774ba559b93c96a4dc4cb0e20eba05a1ff404c9b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:28 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:49:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a705d77fc05da36aa7a1f8f5edb42ad0a278354d7818a46aa366c08c05a9a6`  
		Last Modified: Fri, 13 Oct 2023 20:50:26 GMT  
		Size: 5.6 MB (5606755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be03a937e4af6607f76e748896ccb9bef922488c0ef296120d5170af713977`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516a13f6149cde95784c4dda86214c8e6f629d8b54e67daada10eaedbf16495`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:eb82136d1b0694facbb0e165c28bc2b2b3e43a7207c374c40f14adcdd9fe6a5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8498721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed722d660c639a4623ea7c313732b1214276b7a49aba5feb382c777e952fb3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:33 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:57:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c49c2f4ef415f61afc8f8767700f415271abad05a93c86409223f1ffb582208`  
		Last Modified: Fri, 13 Oct 2023 20:58:52 GMT  
		Size: 5.6 MB (5597814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18deea0b99d1bfaa5737ee833ffc88a535378e7a3386666be65db239e9a797a8`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3671dc5372433df623beb235abc94e688e644e85f86d0347b179526fd165a9c`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:bf7b9a4e1a05493d11d86fc493d67ebf11625e7eff0ee5afd733ae6ccab82556
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8740997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1560dbaf5cdd6a5be38a9524c91d39c8753eb99151610fdfc2fb16b46729d899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:49 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:51 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fe93b371732f5508e482212d76c6956399d79b2ae4994aea9ba1b8fd2e4e9`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 5.4 MB (5408164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bf467ad52a7ee8fe861954ccf4a8a2d09502bbb044dc43820d41608e2711f`  
		Last Modified: Fri, 13 Oct 2023 20:41:28 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc00028abee22a182dd921dc31227b33b33bd7f21227966a71df41bd97cfad08`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:5f2553496dc3b061b01d6c71cc80555740c68717e704288786e7cdb2a58a5bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b12208fb5460efe7e1b62e0c46251c3a1daad5ee716d2705538fd4389c22386a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109797099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2ca8c21a3ef708b1404687d739e38876f4ee7b5bdb23b6bcf873e39d9468ae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:21:13 GMT
RUN cmd /S /C #(nop) COPY file:00bfb4e63864da2c3a8640dc6372df1a1a5dae2d055af3e9d7902b58c0fcde95 in C:\nats-server.exe 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:16 GMT
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
	-	`sha256:4db95068357ee7ae4d2b01d73f339f6beb88bcb4cc1c6d1fdbf47adaf4a83084`  
		Last Modified: Fri, 13 Oct 2023 20:22:45 GMT  
		Size: 5.3 MB (5326094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a669a99c0401b659048d6aefa3257d64d18e4e73d16f1a7f23c7ca16904bef23`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ceeae736fe5ff6bea48a378d2dee9b4f5b515e62be43a6dbc5bf79f538744b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052d84a390e34e3943d4c689fdb1a58bde31d61ea65eb60ef264502597b9099a`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14acdd2d288c743ff91da082ce23136b8977cbf691b19ba5c9fdadb5724d4e4b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:5f2553496dc3b061b01d6c71cc80555740c68717e704288786e7cdb2a58a5bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b12208fb5460efe7e1b62e0c46251c3a1daad5ee716d2705538fd4389c22386a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109797099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2ca8c21a3ef708b1404687d739e38876f4ee7b5bdb23b6bcf873e39d9468ae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:21:13 GMT
RUN cmd /S /C #(nop) COPY file:00bfb4e63864da2c3a8640dc6372df1a1a5dae2d055af3e9d7902b58c0fcde95 in C:\nats-server.exe 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:16 GMT
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
	-	`sha256:4db95068357ee7ae4d2b01d73f339f6beb88bcb4cc1c6d1fdbf47adaf4a83084`  
		Last Modified: Fri, 13 Oct 2023 20:22:45 GMT  
		Size: 5.3 MB (5326094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a669a99c0401b659048d6aefa3257d64d18e4e73d16f1a7f23c7ca16904bef23`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ceeae736fe5ff6bea48a378d2dee9b4f5b515e62be43a6dbc5bf79f538744b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052d84a390e34e3943d4c689fdb1a58bde31d61ea65eb60ef264502597b9099a`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14acdd2d288c743ff91da082ce23136b8977cbf691b19ba5c9fdadb5724d4e4b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:c7386cf07382c8b8bc8112303c10b0888d7183e75df844270bf95f3c6278d146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d690406b91f8f4c855dc0dce4e5fc96b52394c84e1deb4db4ac3e3b76863e84d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037672217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896c6a11456cb73f29bb84dde01d5762f95793acbde0ca10557e869d13607af`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:18:14 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:18:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.23/nats-server-v2.9.23-windows-amd64.zip
# Fri, 13 Oct 2023 20:18:16 GMT
ENV NATS_SERVER_SHASUM=68604d0df9f276bf7773f67fd95267ee129662e7872e270707c852f056276db7
# Fri, 13 Oct 2023 20:19:16 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:20:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:20:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:20:59 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c067d6d13f4a842896f054d8faf94b4f19d2b893e661eb83255fef9f97427b51`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86b90b57ef0ff96cfb84a6b2299fafdcb441f4cdf20444bd6d8e08d30d1077`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa67c6b32d2f520576f3cea8105a67acf43b87fb0b517485d0cafd2a93b83c1`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6050ec1bea96c503aab3a151f6c042e3c749195a3122a52843aceaf051ea376`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 449.8 KB (449761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87861da09dbd687e92f0b2fc6e3aeb110c75a58b1db499da489a19c0b555e34e`  
		Last Modified: Fri, 13 Oct 2023 20:22:26 GMT  
		Size: 5.6 MB (5618675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26716f4d0d22b10eea724fee02faa1237634263791c2a6dbc73faad09c93eebd`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b00496fe874c2269a71e1b085bbb727355b0d29893a6fe274a92cf3c482927`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e3adaebf8fe75f24dcc73fe777e29cf10016f2516280fe6f7e64c2dc9d6a04`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0adb5e427986ffd48e87604a9b778cee3f62bd8c75f80840e00ccb4ffdead`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:c7386cf07382c8b8bc8112303c10b0888d7183e75df844270bf95f3c6278d146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d690406b91f8f4c855dc0dce4e5fc96b52394c84e1deb4db4ac3e3b76863e84d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037672217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896c6a11456cb73f29bb84dde01d5762f95793acbde0ca10557e869d13607af`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:18:14 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:18:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.23/nats-server-v2.9.23-windows-amd64.zip
# Fri, 13 Oct 2023 20:18:16 GMT
ENV NATS_SERVER_SHASUM=68604d0df9f276bf7773f67fd95267ee129662e7872e270707c852f056276db7
# Fri, 13 Oct 2023 20:19:16 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:20:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:20:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:20:59 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c067d6d13f4a842896f054d8faf94b4f19d2b893e661eb83255fef9f97427b51`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86b90b57ef0ff96cfb84a6b2299fafdcb441f4cdf20444bd6d8e08d30d1077`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa67c6b32d2f520576f3cea8105a67acf43b87fb0b517485d0cafd2a93b83c1`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6050ec1bea96c503aab3a151f6c042e3c749195a3122a52843aceaf051ea376`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 449.8 KB (449761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87861da09dbd687e92f0b2fc6e3aeb110c75a58b1db499da489a19c0b555e34e`  
		Last Modified: Fri, 13 Oct 2023 20:22:26 GMT  
		Size: 5.6 MB (5618675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26716f4d0d22b10eea724fee02faa1237634263791c2a6dbc73faad09c93eebd`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b00496fe874c2269a71e1b085bbb727355b0d29893a6fe274a92cf3c482927`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e3adaebf8fe75f24dcc73fe777e29cf10016f2516280fe6f7e64c2dc9d6a04`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0adb5e427986ffd48e87604a9b778cee3f62bd8c75f80840e00ccb4ffdead`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.23` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-alpine`

```console
$ docker pull nats@sha256:664aad0be228e0f38246ff04e7dcb84487b33dc8f3cc13e5ff09c77de0fc3245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.23-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2493aea2c3d9f0cbd5842f9e7cf0ae1cca872dcab55b986634737fc0bea98c67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9273216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7989a8298522649a1adb3ca614130cb34f8bf861930fdaae0cf9cf7fe777a8ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:12 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:14 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86325e476145954afe4454d6a34d1a8ee010d39db18e02ccc18f3173c1f76c5`  
		Last Modified: Fri, 13 Oct 2023 20:21:48 GMT  
		Size: 5.9 MB (5870249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e197bedf457b6e20573397488cb470629dbb34103b46f2e8afc0fdf0a04aac`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fee3723b24b5f8fe02d83f43f4c5e58a7c7d7e9ad295e1090b5c1121de96ad`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:043a42240b54eff4efa7d2e58782a319fbfb8ccfb9014a94ad57ee293f4710bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8753049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992beb8b085db72a7b6711b774ba559b93c96a4dc4cb0e20eba05a1ff404c9b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:28 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:49:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a705d77fc05da36aa7a1f8f5edb42ad0a278354d7818a46aa366c08c05a9a6`  
		Last Modified: Fri, 13 Oct 2023 20:50:26 GMT  
		Size: 5.6 MB (5606755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be03a937e4af6607f76e748896ccb9bef922488c0ef296120d5170af713977`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516a13f6149cde95784c4dda86214c8e6f629d8b54e67daada10eaedbf16495`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:eb82136d1b0694facbb0e165c28bc2b2b3e43a7207c374c40f14adcdd9fe6a5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8498721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed722d660c639a4623ea7c313732b1214276b7a49aba5feb382c777e952fb3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:33 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:57:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c49c2f4ef415f61afc8f8767700f415271abad05a93c86409223f1ffb582208`  
		Last Modified: Fri, 13 Oct 2023 20:58:52 GMT  
		Size: 5.6 MB (5597814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18deea0b99d1bfaa5737ee833ffc88a535378e7a3386666be65db239e9a797a8`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3671dc5372433df623beb235abc94e688e644e85f86d0347b179526fd165a9c`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:bf7b9a4e1a05493d11d86fc493d67ebf11625e7eff0ee5afd733ae6ccab82556
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8740997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1560dbaf5cdd6a5be38a9524c91d39c8753eb99151610fdfc2fb16b46729d899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:49 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:51 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fe93b371732f5508e482212d76c6956399d79b2ae4994aea9ba1b8fd2e4e9`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 5.4 MB (5408164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bf467ad52a7ee8fe861954ccf4a8a2d09502bbb044dc43820d41608e2711f`  
		Last Modified: Fri, 13 Oct 2023 20:41:28 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc00028abee22a182dd921dc31227b33b33bd7f21227966a71df41bd97cfad08`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-alpine3.18`

```console
$ docker pull nats@sha256:664aad0be228e0f38246ff04e7dcb84487b33dc8f3cc13e5ff09c77de0fc3245
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.23-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2493aea2c3d9f0cbd5842f9e7cf0ae1cca872dcab55b986634737fc0bea98c67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9273216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7989a8298522649a1adb3ca614130cb34f8bf861930fdaae0cf9cf7fe777a8ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:12 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:20:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:14 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:14 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:15 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86325e476145954afe4454d6a34d1a8ee010d39db18e02ccc18f3173c1f76c5`  
		Last Modified: Fri, 13 Oct 2023 20:21:48 GMT  
		Size: 5.9 MB (5870249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e197bedf457b6e20573397488cb470629dbb34103b46f2e8afc0fdf0a04aac`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fee3723b24b5f8fe02d83f43f4c5e58a7c7d7e9ad295e1090b5c1121de96ad`  
		Last Modified: Fri, 13 Oct 2023 20:21:47 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:043a42240b54eff4efa7d2e58782a319fbfb8ccfb9014a94ad57ee293f4710bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8753049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992beb8b085db72a7b6711b774ba559b93c96a4dc4cb0e20eba05a1ff404c9b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:28 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:49:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a705d77fc05da36aa7a1f8f5edb42ad0a278354d7818a46aa366c08c05a9a6`  
		Last Modified: Fri, 13 Oct 2023 20:50:26 GMT  
		Size: 5.6 MB (5606755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17be03a937e4af6607f76e748896ccb9bef922488c0ef296120d5170af713977`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8516a13f6149cde95784c4dda86214c8e6f629d8b54e67daada10eaedbf16495`  
		Last Modified: Fri, 13 Oct 2023 20:50:25 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:eb82136d1b0694facbb0e165c28bc2b2b3e43a7207c374c40f14adcdd9fe6a5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8498721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed722d660c639a4623ea7c313732b1214276b7a49aba5feb382c777e952fb3f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:33 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:57:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:36 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:36 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c49c2f4ef415f61afc8f8767700f415271abad05a93c86409223f1ffb582208`  
		Last Modified: Fri, 13 Oct 2023 20:58:52 GMT  
		Size: 5.6 MB (5597814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18deea0b99d1bfaa5737ee833ffc88a535378e7a3386666be65db239e9a797a8`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3671dc5372433df623beb235abc94e688e644e85f86d0347b179526fd165a9c`  
		Last Modified: Fri, 13 Oct 2023 20:58:51 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:bf7b9a4e1a05493d11d86fc493d67ebf11625e7eff0ee5afd733ae6ccab82556
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8740997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1560dbaf5cdd6a5be38a9524c91d39c8753eb99151610fdfc2fb16b46729d899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:49 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:39:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='8c62d1c9f15651a22c4adaa9bfacffc3ade97f998bd5a5557074576ecf34bba2' ;; 		armhf) natsArch='arm6'; sha256='93c252b9ac70f22d6fbbc0bc8bc8624287dd0955a6c3bb5057e576af9c7d355a' ;; 		armv7) natsArch='arm7'; sha256='08e0c2a1b0d69135070464dce735038c99a882daadd1e3eaae050eacb61eac4c' ;; 		x86_64) natsArch='amd64'; sha256='8a52b6b4a0337d3c58ee70888bf605cc732d792d9babe6bc9c984a1967aff15f' ;; 		x86) natsArch='386'; sha256='102844ff97e19ab81728030e6a97e7cd7a228e63c07cc9132590d0193d3283d9' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:51 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248fe93b371732f5508e482212d76c6956399d79b2ae4994aea9ba1b8fd2e4e9`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 5.4 MB (5408164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8bf467ad52a7ee8fe861954ccf4a8a2d09502bbb044dc43820d41608e2711f`  
		Last Modified: Fri, 13 Oct 2023 20:41:28 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc00028abee22a182dd921dc31227b33b33bd7f21227966a71df41bd97cfad08`  
		Last Modified: Fri, 13 Oct 2023 20:41:29 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-linux`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.23-linux` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-nanoserver`

```console
$ docker pull nats@sha256:5f2553496dc3b061b01d6c71cc80555740c68717e704288786e7cdb2a58a5bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.23-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b12208fb5460efe7e1b62e0c46251c3a1daad5ee716d2705538fd4389c22386a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109797099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2ca8c21a3ef708b1404687d739e38876f4ee7b5bdb23b6bcf873e39d9468ae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:21:13 GMT
RUN cmd /S /C #(nop) COPY file:00bfb4e63864da2c3a8640dc6372df1a1a5dae2d055af3e9d7902b58c0fcde95 in C:\nats-server.exe 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:16 GMT
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
	-	`sha256:4db95068357ee7ae4d2b01d73f339f6beb88bcb4cc1c6d1fdbf47adaf4a83084`  
		Last Modified: Fri, 13 Oct 2023 20:22:45 GMT  
		Size: 5.3 MB (5326094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a669a99c0401b659048d6aefa3257d64d18e4e73d16f1a7f23c7ca16904bef23`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ceeae736fe5ff6bea48a378d2dee9b4f5b515e62be43a6dbc5bf79f538744b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052d84a390e34e3943d4c689fdb1a58bde31d61ea65eb60ef264502597b9099a`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14acdd2d288c743ff91da082ce23136b8977cbf691b19ba5c9fdadb5724d4e4b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-nanoserver-1809`

```console
$ docker pull nats@sha256:5f2553496dc3b061b01d6c71cc80555740c68717e704288786e7cdb2a58a5bc9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.23-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b12208fb5460efe7e1b62e0c46251c3a1daad5ee716d2705538fd4389c22386a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109797099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da2ca8c21a3ef708b1404687d739e38876f4ee7b5bdb23b6bcf873e39d9468ae`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:21:13 GMT
RUN cmd /S /C #(nop) COPY file:00bfb4e63864da2c3a8640dc6372df1a1a5dae2d055af3e9d7902b58c0fcde95 in C:\nats-server.exe 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:21:14 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:15 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:16 GMT
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
	-	`sha256:4db95068357ee7ae4d2b01d73f339f6beb88bcb4cc1c6d1fdbf47adaf4a83084`  
		Last Modified: Fri, 13 Oct 2023 20:22:45 GMT  
		Size: 5.3 MB (5326094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a669a99c0401b659048d6aefa3257d64d18e4e73d16f1a7f23c7ca16904bef23`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ceeae736fe5ff6bea48a378d2dee9b4f5b515e62be43a6dbc5bf79f538744b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052d84a390e34e3943d4c689fdb1a58bde31d61ea65eb60ef264502597b9099a`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14acdd2d288c743ff91da082ce23136b8977cbf691b19ba5c9fdadb5724d4e4b`  
		Last Modified: Fri, 13 Oct 2023 20:22:43 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-scratch`

```console
$ docker pull nats@sha256:e555c1ca5c508ec2290d709105a6cb379511df462211a40343c43356f1c5c09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.23-scratch` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.23-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-windowsservercore`

```console
$ docker pull nats@sha256:c7386cf07382c8b8bc8112303c10b0888d7183e75df844270bf95f3c6278d146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.23-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d690406b91f8f4c855dc0dce4e5fc96b52394c84e1deb4db4ac3e3b76863e84d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037672217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896c6a11456cb73f29bb84dde01d5762f95793acbde0ca10557e869d13607af`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:18:14 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:18:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.23/nats-server-v2.9.23-windows-amd64.zip
# Fri, 13 Oct 2023 20:18:16 GMT
ENV NATS_SERVER_SHASUM=68604d0df9f276bf7773f67fd95267ee129662e7872e270707c852f056276db7
# Fri, 13 Oct 2023 20:19:16 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:20:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:20:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:20:59 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c067d6d13f4a842896f054d8faf94b4f19d2b893e661eb83255fef9f97427b51`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86b90b57ef0ff96cfb84a6b2299fafdcb441f4cdf20444bd6d8e08d30d1077`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa67c6b32d2f520576f3cea8105a67acf43b87fb0b517485d0cafd2a93b83c1`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6050ec1bea96c503aab3a151f6c042e3c749195a3122a52843aceaf051ea376`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 449.8 KB (449761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87861da09dbd687e92f0b2fc6e3aeb110c75a58b1db499da489a19c0b555e34e`  
		Last Modified: Fri, 13 Oct 2023 20:22:26 GMT  
		Size: 5.6 MB (5618675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26716f4d0d22b10eea724fee02faa1237634263791c2a6dbc73faad09c93eebd`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b00496fe874c2269a71e1b085bbb727355b0d29893a6fe274a92cf3c482927`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e3adaebf8fe75f24dcc73fe777e29cf10016f2516280fe6f7e64c2dc9d6a04`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0adb5e427986ffd48e87604a9b778cee3f62bd8c75f80840e00ccb4ffdead`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.23-windowsservercore-1809`

```console
$ docker pull nats@sha256:c7386cf07382c8b8bc8112303c10b0888d7183e75df844270bf95f3c6278d146
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.23-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d690406b91f8f4c855dc0dce4e5fc96b52394c84e1deb4db4ac3e3b76863e84d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037672217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1896c6a11456cb73f29bb84dde01d5762f95793acbde0ca10557e869d13607af`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:18:14 GMT
ENV NATS_SERVER=2.9.23
# Fri, 13 Oct 2023 20:18:15 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.23/nats-server-v2.9.23-windows-amd64.zip
# Fri, 13 Oct 2023 20:18:16 GMT
ENV NATS_SERVER_SHASUM=68604d0df9f276bf7773f67fd95267ee129662e7872e270707c852f056276db7
# Fri, 13 Oct 2023 20:19:16 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:20:58 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:20:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:20:59 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:21:00 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:21:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c067d6d13f4a842896f054d8faf94b4f19d2b893e661eb83255fef9f97427b51`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed86b90b57ef0ff96cfb84a6b2299fafdcb441f4cdf20444bd6d8e08d30d1077`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa67c6b32d2f520576f3cea8105a67acf43b87fb0b517485d0cafd2a93b83c1`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6050ec1bea96c503aab3a151f6c042e3c749195a3122a52843aceaf051ea376`  
		Last Modified: Fri, 13 Oct 2023 20:22:27 GMT  
		Size: 449.8 KB (449761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87861da09dbd687e92f0b2fc6e3aeb110c75a58b1db499da489a19c0b555e34e`  
		Last Modified: Fri, 13 Oct 2023 20:22:26 GMT  
		Size: 5.6 MB (5618675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26716f4d0d22b10eea724fee02faa1237634263791c2a6dbc73faad09c93eebd`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.9 KB (1941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b00496fe874c2269a71e1b085bbb727355b0d29893a6fe274a92cf3c482927`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e3adaebf8fe75f24dcc73fe777e29cf10016f2516280fe6f7e64c2dc9d6a04`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd0adb5e427986ffd48e87604a9b778cee3f62bd8c75f80840e00ccb4ffdead`  
		Last Modified: Fri, 13 Oct 2023 20:22:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:da1eb7478d24a313509338be67dd17478870881a21eb30d0246d6a82e91266d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:2cceb1f3fa7b15611e166ed479dd90d3e43b8d46cb776d08f64e05deb200be68
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9498416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a57a41cbb09fe1a60b56fd7522328ad6c507b968b2837855dba4d6661e84806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:20:05 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:20:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:20:08 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:20:08 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:20:08 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ad1a616f2a37d0761343518ccdc80755abd01cb3c30a49c3a328adc0d7024c`  
		Last Modified: Fri, 13 Oct 2023 20:21:25 GMT  
		Size: 6.1 MB (6095446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3ded5aac5d1e1475aec9d0629cd78f96b816735bada84e67b6ee7abeafcaa7`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5407fa2efd19d981d3f8ffcc0cde53637fa5fcd5cccbba08976c8db248aee5`  
		Last Modified: Fri, 13 Oct 2023 20:21:23 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:c396810cff0b8e5d376956733815f1821a74b6c5a32758a3b7f4814afa54f660
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8959561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:457fab83639c9d351944ed83d25e70d9fdecda349419acd221d702f136e514a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:49:23 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:49:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:49:26 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:49:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:49:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61241071cebda9cba981b7b82f393e119b961bd9159bf55dcdba1c4624e45917`  
		Last Modified: Fri, 13 Oct 2023 20:50:04 GMT  
		Size: 5.8 MB (5813268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a337d1a669a446adc02d1d8002392edf0fe2d8138ef94a0e50ee7530ec685fe4`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b037061c6ffd9f106c296b4de2e1020665e9f20af8504311b688fbf579ec44`  
		Last Modified: Fri, 13 Oct 2023 20:50:02 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:17c05176e65bf9d0e1491927694e3044a595cb8b8e4bb2dea59ebcca6604a15f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d36339c31362689fb85865c6dd5463c41fbc8316ead741ca7cf2bd7aa7d31e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:57:28 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:57:31 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:57:31 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d4d62a2fc0e535870d4eb68884f7c44422fac7850ed219352cb3b6f323195a`  
		Last Modified: Fri, 13 Oct 2023 20:58:30 GMT  
		Size: 5.8 MB (5803745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1309051fb0c589da4d478edb5890d87ec73851f7d22b94f676eb80a98eece7`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4f9000751a913e3d4861bb2e51a86d81df3a1822e8439e3c67216216ca29cb`  
		Last Modified: Fri, 13 Oct 2023 20:58:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:10622e60a928a676f6bd678c05fd8146ec12e0ce1a02063af044dcbb6983b55e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9002000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea617ccf0da02c9e88f244b2dccd65610b1b4fd6b7344bb61b01de68426f539d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 13 Oct 2023 20:39:43 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='924a92491f549be8e8d51d56fc0cd211e8326933b9e7c2bbd31af0fdc7f15240' ;; 		armhf) natsArch='arm6'; sha256='dc8cfc756af14cda3c754ebfbe942616f7e3e65b8d846e7a34f5de2c55612a9d' ;; 		armv7) natsArch='arm7'; sha256='f8e4cf88d50800650b0fed026e776d8ca7eace6b0cbc4762beca7d0f3590ba00' ;; 		x86_64) natsArch='amd64'; sha256='a5587b04062a9cf117ec13aea5cb60cf4cd2e644be8c44628d85b5f4dfc19ab6' ;; 		x86) natsArch='386'; sha256='e8a1a521aeeef68abf2b1bd3baf3f359a073c25cef4f87aa505a49c1b0920e90' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 13 Oct 2023 20:39:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 13 Oct 2023 20:39:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 20:39:46 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89779f99904600f0b8257e364b4b34fbc2dfada2a75d6ef94cb9202a0b63b2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:03 GMT  
		Size: 5.7 MB (5669169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b37a3e5cd62562515d46192516aa3e3c3549500a7962fa65c0a37d0e143e2f`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f4fb413d4d2c0b6f57336bc01227dfe8bbef8a217d95c5d06496241c8c3d84`  
		Last Modified: Fri, 13 Oct 2023 20:41:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:a7896fa3caaffacae323f1777007005298abd0524c6aced0af5c48a39e49062f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:1665196d1eff76b899dcfc99c16973dd5e7747401ecc8e1a746c8d1f62200481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5247111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe6b84d14d2886336d994782eca00af921f74810c30ae727bb9b4803fb296adb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:71487567f54b75938083a2680d411bd9e194b037c12b743a3c280c58abd7e82f in /nats-server 
# Fri, 13 Oct 2023 20:20:46 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:46 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:46 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:46 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5d153758a0dd20c137d358179ec27f8aca298056d0b26005f90208c882f0c7fa`  
		Last Modified: Fri, 13 Oct 2023 20:22:03 GMT  
		Size: 5.2 MB (5246604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8a0aaec4b4f43b0da805ca5537d4c575d1b8781b8e392628b99a6d6e68b5`  
		Last Modified: Fri, 13 Oct 2023 20:22:07 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:a8e5748f25ba2b48e9cf9a93b790beaa40e7fa2ce5493c7adfd2c9135f2cf93e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4983319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5dfe1fe3336905b38f5458891c7cf78baacff67a5caef2b82f27bfe9d59479`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:a99ff6735b1292770195e5dfe0e7f8a56bae939bfb272c8cbdfb47e7ba6c4828 in /nats-server 
# Fri, 13 Oct 2023 20:49:37 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:37 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:37 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:37 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:217c24d6cc08c267f56e5da2ce4e101011c47ccc55a86d28c979a19ebcb92d1e`  
		Last Modified: Fri, 13 Oct 2023 20:50:41 GMT  
		Size: 5.0 MB (4982809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdd0760fe43c91213d66bc7c8129ce5845aa6f399d019b7320017c515506a0a`  
		Last Modified: Fri, 13 Oct 2023 20:50:40 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:fbb684ac1d802e889557b1b925a6ca25fc47557530d8b2ce3ff8250063d29ad1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab4ec32890f6a0cd584bc3ee224b16692923488ad8903fbfa36222533a879657`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:c45665aaa0d25bdd0098d10b44c0de8efea234c8bb8ca8d2159b85284914acec in /nats-server 
# Fri, 13 Oct 2023 20:57:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:57:56 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:57:56 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a4d0acc6fe81e822f8d7b966098f56b50e69fda2eaab5ba79292315f68bc3a00`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 5.0 MB (4975782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136cd05f311d345bdd24e413e4236179806020db9326d336daedf4ddd2aff099`  
		Last Modified: Fri, 13 Oct 2023 20:59:06 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:948b11163b9a928af28fa5221ed3adffda05fcf2fa8eee86885d3b01899663c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4784169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bec03642400d44e9de3558e19df4239f7664786fae6a466b8f1b5b978d2a24fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:75276c307f8eba0e9701c41a06bc7811acfb74142d0dee0a37dfb289dfda3db1 in /nats-server 
# Fri, 13 Oct 2023 20:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:26 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c50a270bdf1d14f1505fe9a625df2c74a90941d423db84eb62da12b3b6c813a4`  
		Last Modified: Fri, 13 Oct 2023 20:42:09 GMT  
		Size: 4.8 MB (4783661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f772c8dffdfc71ead54f31a3d3198c931e5d4b5a3f8b4938337b31e0f8be9479`  
		Last Modified: Fri, 13 Oct 2023 20:42:08 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4974; amd64

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

## `nats:linux`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:986279fb525b5e5f784850efad3c95571eb0191ffb35b349668d2a6397c19ef0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:nanoserver` - windows version 10.0.17763.4974; amd64

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

## `nats:scratch`

```console
$ docker pull nats@sha256:2ba972f43bc72b7585c6b4c0d0556fb003fbafd279a1403ca7ed08f0c832ad89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:1f5fd4c2667baa8706a01a5142ebfc7da4e54b40e836f6023c542e98a05d3633
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5473290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a627248b7b1c4d5c4c34458f79a9a3c8c3a9376ce38d013717a4f7c46e1be7c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:8348bba8fefe594deaff23a8e8d05c5fe8b20634309016cd157744d47b01e751 in /nats-server 
# Fri, 13 Oct 2023 20:20:56 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:20:57 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:20:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:20:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4f6c5282fce6f13ac2ac3b630b77fdf0eedb5f5bc51022facee92dfab0158a59`  
		Last Modified: Fri, 13 Oct 2023 20:22:22 GMT  
		Size: 5.5 MB (5472781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccfbb89f4006d0b4c994aef2a537d6009ce16bd56e9ce65e5c3eb9bafb12bf`  
		Last Modified: Fri, 13 Oct 2023 20:22:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:8e3600e43a3f1ae04ce8919623b7fb401c41946c36f1d784b06ecdb0d019378f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5190587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f1db5cabe7cb404f4a0e8801ffde3bdf44b2495fc041742f8cae7beda61db2e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:8dacc397b23c5135d4de7bf3f45ab027ff2c86caa3aad1e15af7be5f04d445ad in /nats-server 
# Fri, 13 Oct 2023 20:49:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:49:40 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:49:40 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:49:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:19ec1fbe1f08c131312370f7ea60d44458bc6ab6071134407e6e4ae56aabd35c`  
		Last Modified: Fri, 13 Oct 2023 20:50:56 GMT  
		Size: 5.2 MB (5190079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c9aea24f990257539ff0ecab608af2e33941da1a649512ea4fbafd630fb26`  
		Last Modified: Fri, 13 Oct 2023 20:50:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:e2e0f731700bd5cb5b101e61d8514a11fdde9a6b09d08ab369b78a3c9a1a64c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5181141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d72314affa3f39d032c3fa47bf1ed0f523570341564517b230c99f67bff4ea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:58:05 GMT
COPY file:7c0c4073772c48f768f2e91bfa31b0c5d556879520ae0ea32fc6935bf412dc00 in /nats-server 
# Fri, 13 Oct 2023 20:58:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:58:06 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:58:06 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:58:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:31d2c5aa698d33f10bc977a89c17f3061f738bcf64b2a5da150959029f61cf0d`  
		Last Modified: Fri, 13 Oct 2023 20:59:21 GMT  
		Size: 5.2 MB (5180631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdb6d579e3778a5b42802b9088e8b0fe812a0dfb2c10f581a1f55a675e70f`  
		Last Modified: Fri, 13 Oct 2023 20:59:20 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b50690e08f9d00c61df3c20b0ad31c846f48059d9d539cb6846c5de84ac47893
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5045078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:614fd2312c018384c8226cd53fedafd182889df8b583a37290092e813dac2954`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:19248ff038b76e97dd2ecca66b4c7405f937e42b4333f3145ccd80bf7163d961 in /nats-server 
# Fri, 13 Oct 2023 20:40:36 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 13 Oct 2023 20:40:36 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:40:36 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 13 Oct 2023 20:40:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e53370f26f56fa38d3df795930e6aff84ff23630dcb11457890c5a66f697b145`  
		Last Modified: Fri, 13 Oct 2023 20:42:28 GMT  
		Size: 5.0 MB (5044570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc37154fa1c7115cc01b946241357166988b0297233bc5b43296359a208b619`  
		Last Modified: Fri, 13 Oct 2023 20:42:27 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:36def1f4c1d5a7a2038f81e533bb5dd5ddaf79e195b2083651de412b8a09e3ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:b96058f0abbf858d83160210231c7c2a0bed54c8fcda52342133dfc9f0ad258a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037938189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:876c267b5fecf8ba8da6cfc10f1952395f0aa829d899d6a6f789b46423d6cf74`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Fri, 13 Oct 2023 20:15:06 GMT
ENV NATS_SERVER=2.10.3
# Fri, 13 Oct 2023 20:15:07 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.3/nats-server-v2.10.3-windows-amd64.zip
# Fri, 13 Oct 2023 20:15:08 GMT
ENV NATS_SERVER_SHASUM=4c1d9537562134450e2332dc1561d1ab64beb45fc82e01bc89b9403e3f6d680f
# Fri, 13 Oct 2023 20:16:10 GMT
RUN Set-PSDebug -Trace 2
# Fri, 13 Oct 2023 20:17:53 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Fri, 13 Oct 2023 20:17:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 13 Oct 2023 20:17:55 GMT
EXPOSE 4222 6222 8222
# Fri, 13 Oct 2023 20:17:55 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 13 Oct 2023 20:17:56 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2c59764edeb5a9eb73e90ad90f0df91e731dac208e75bb8d3045985a35b46`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f059f74917a94519977101cdcd91e6eca57a387d5d53147d5b96fa722552e0`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79fb62c7bf71d873fbed15e0344a8f6976b86f16d41276ab009108e9b918a855`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad74f3edaa649c29cd7ad4508d28d0e25979664c3a3198452019a82661e026`  
		Last Modified: Fri, 13 Oct 2023 20:21:54 GMT  
		Size: 454.6 KB (454615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c7895231c0ab196b12f1327f4487a221bbd9d87e0011eb693d7d2bd2a206e`  
		Last Modified: Fri, 13 Oct 2023 20:21:53 GMT  
		Size: 5.9 MB (5879724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc539d58ea38523dd5da406ce195e9af73cc0b40a406cdad13ce87eb641d8308`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 2.0 KB (2001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f34090a57ba21eb445112261cc5e97b649674a537ea643c543eb7d5d6a3ba4c`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072215f5155480305c6d5df8627c9b86f41581c8e2cd3d6a5d31288f6b4b414`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36d40fb089c2f6b3e8ab73302ca5e82c97115acc8c4497d931c6ca9c39cc2b3`  
		Last Modified: Fri, 13 Oct 2023 20:21:52 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
