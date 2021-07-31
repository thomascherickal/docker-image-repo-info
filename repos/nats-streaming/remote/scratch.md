## `nats-streaming:scratch`

```console
$ docker pull nats-streaming@sha256:192498e150efb79ad37515df195d730d5c0bbeaf640740ddae2e6d8e54325602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:scratch` - linux; amd64

```console
$ docker pull nats-streaming@sha256:ba1be2cd913a1e9f1ffc9445e5c04c169db333819beb7204deb3bc7c29fde5a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6800613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12f2d32e0c9a23e5a9a5cb19c8b1404a9cc7af17915e33eabb71e55767848df7`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 05:47:24 GMT
COPY file:bbdef008b65f574a4e4593641e45dd6cdff5e8261d06d8f3959963f686dcdb78 in /nats-streaming-server 
# Wed, 02 Jun 2021 05:47:24 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 05:47:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 05:47:24 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:afa0998a9989cfec22c4ad772da3ca685ea7ccf963253ff9c27edf33a00d49c6`  
		Last Modified: Wed, 02 Jun 2021 05:48:07 GMT  
		Size: 6.8 MB (6800613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0b8d3b4c948e889fc5afd06e6676d2f7d36dcbe96a90b65f0c365cccf152a8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6269700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fab51a53d8819a986c5b3e4f5a010fa64eecbd90977babef20bd96775a32389`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 31 Jul 2021 02:40:37 GMT
COPY file:a4f69de3d07c6870dde4796b4de69a931a699d7e5b6ec30b2f25f6a23d66cb33 in /nats-streaming-server 
# Sat, 31 Jul 2021 02:40:38 GMT
EXPOSE 4222 8222
# Sat, 31 Jul 2021 02:40:38 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 31 Jul 2021 02:40:39 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:8ab135edb380ca588ed7d11dbea1418006a6708ae7ae5effad8d86bcef90198e`  
		Last Modified: Tue, 01 Jun 2021 23:56:26 GMT  
		Size: 6.3 MB (6269700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a6c122176a5ff4bdae9a653ebb1cf3e0672cd240250547b855ae0f8894496225
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 MB (6259769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccaf377f82ea563a543d1a8bcf9a53870f6427a0cacae9f9ad5e46e6c7eabff`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 03:13:19 GMT
COPY file:6e08520addf5d0c5d064e431d76487779d8fd8f4c03f71a72dc4e2c81812a922 in /nats-streaming-server 
# Wed, 02 Jun 2021 03:13:20 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 03:13:20 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 03:13:20 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:887fd90bbdf32bb85ec9e85b63e60eccca791d6c882e30de0c10e6e583ccbb65`  
		Last Modified: Wed, 02 Jun 2021 03:15:02 GMT  
		Size: 6.3 MB (6259769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:scratch` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:bd5a415582b3f1d079d6498c12ea9138d7bde01dcd3a5f5a35a1731edf4c889f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6197708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16d36744f70db176ba94e376a65c5edda55a7167035e7dffdf217e594c1ac283`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 02 Jun 2021 02:14:00 GMT
COPY file:ef2047bb70888b72ef213e68689b3b8ae622cc597cd07b313c26b278418788bd in /nats-streaming-server 
# Wed, 02 Jun 2021 02:14:00 GMT
EXPOSE 4222 8222
# Wed, 02 Jun 2021 02:14:01 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 02 Jun 2021 02:14:01 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:ddf987a265c2be80179a2683a2d725f5a7e9fb477bc5752443a6d955be681a50`  
		Last Modified: Wed, 02 Jun 2021 02:15:07 GMT  
		Size: 6.2 MB (6197708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
