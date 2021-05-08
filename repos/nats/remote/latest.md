## `nats:latest`

```console
$ docker pull nats@sha256:00eb6d907368f5637e0ee0af3f0e1b8135b3bd4a87636d33ed1709201422cb83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1879; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:7a091e96f75533db8948728659c0f8af66231dea1ea53ee30174a89d5e8853f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4239970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2cb2ff23053c8b52e48efca2094f55a8966b73d5921b31266f7c8e4418ca5e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:20:50 GMT
COPY file:4bdc1ffeaec1d05d83ec33452dde470ae9b3088a21aecb0d9cc17c192bb4d530 in /nats-server 
# Sat, 08 May 2021 01:20:50 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:20:50 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:20:50 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:20:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:54f52cf564033f26e5a9d8a902be39964b2ea34278061e77ec6544b446226a4f`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 4.2 MB (4239494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b4184478e7fd696a4b8d30267cccc94e7c88ae45a27ae21cb74af50fe8bd12`  
		Last Modified: Sat, 08 May 2021 01:21:45 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4bfb97de25c270a4855e5be65993baa8fef14263b62e8fff557487e3b8fe347c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3911172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a08334f5f368eed5f45bdffc01bb0ced2589e5c975408b839b737b92413bb6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:05:18 GMT
COPY file:27497700f4bdbb247f8a4730533f7570264ce6c9bf877c6a6bbf2cd5fe33af07 in /nats-server 
# Sat, 08 May 2021 01:05:19 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:05:20 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:05:21 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:05:22 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:475132779eb1af9411626b9af000ccdf0fd9f6abbba63568c27f53b7ea473eb1`  
		Last Modified: Sat, 08 May 2021 01:06:09 GMT  
		Size: 3.9 MB (3910695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6424e0f95160ae0dec6e15ec6b0d514f91fadac8e98bddbb28f0ad117d1580d1`  
		Last Modified: Sat, 08 May 2021 01:06:08 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:9e8a6b04725d2ab13cb475c77ebd7e4e196f8055d58f6c458fd4cd20a38d7eab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a24176a676293592dd3b18523e65c42587c782397aa3c9be90f05c4209e084`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:08:24 GMT
COPY file:25eda1378c8897f62c5f38cb184ecbee5e30c2238a48dd4b6170e466c843e759 in /nats-server 
# Sat, 08 May 2021 01:08:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:08:27 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:08:27 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:08:28 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:539e278b5e351d1f1334043c2bbf4d597b62573d1bb3e846d70f5cda956ecf5e`  
		Last Modified: Sat, 08 May 2021 01:09:10 GMT  
		Size: 3.9 MB (3905232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d897fe50920c59f14d6c2120d8db29804a87bb1046bb09291e52e63de08b538`  
		Last Modified: Sat, 08 May 2021 01:09:09 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d09e08717def108aba923a932183d6d8653145669ee6ffd70a5a1c1c3700b33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3882719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d81ea2a01da1e801a146e009aa78d763b8f1f5e8d2dbbe19d1ce98529a3e7b1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 08 May 2021 01:50:21 GMT
COPY file:5a6dc51a9269cfa2c34a63ccece2735f1f2754035657c0e141fb58e50874fbd4 in /nats-server 
# Sat, 08 May 2021 01:50:23 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Sat, 08 May 2021 01:50:24 GMT
EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:50:25 GMT
ENTRYPOINT ["/nats-server"]
# Sat, 08 May 2021 01:50:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c58d26889c72b98b663ca6cc673debbe5f1120d085d0eb2e36230cc13710da38`  
		Last Modified: Sat, 08 May 2021 01:51:15 GMT  
		Size: 3.9 MB (3882242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee2e94e93b8215091b3627ad0972d3f6f29aefda82620a4b7475fe57b7e85b`  
		Last Modified: Sat, 08 May 2021 01:51:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
