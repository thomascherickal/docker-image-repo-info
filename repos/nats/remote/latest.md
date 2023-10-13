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
