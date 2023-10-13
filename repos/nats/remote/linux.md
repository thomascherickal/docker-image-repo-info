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
