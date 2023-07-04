## `debian:experimental-20230703`

```console
$ docker pull debian@sha256:2ad4cfb7a4b5d479fe607a50c2a50ff9fa9607f3797f8ba09028ef5705edff66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; riscv64

### `debian:experimental-20230703` - linux; arm variant v5

```console
$ docker pull debian@sha256:8c0a40eb00289d699534f5b060d1c9e9bb61b508c6d5fc662606ba1f250b07c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47322694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:883bff7d7307e93e117c0640650f6717d50ba33c539fecd83d3e1638c5d7f5a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:50:15 GMT
ADD file:0d73a7183a38c56858e61e53f0c64ae6eaf9d58311df1be7af3b37f1e1769dd2 in / 
# Tue, 04 Jul 2023 00:50:16 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 00:50:26 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:eb46e2b513bf023b4297bc46404f96d3a604f8f913dffe3d1f9e5c5c530e9caf`  
		Last Modified: Tue, 04 Jul 2023 00:55:44 GMT  
		Size: 47.3 MB (47322476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b079d533182e62457871a1cdecd8b7307dda1c497fda642b534f1738b904b1aa`  
		Last Modified: Tue, 04 Jul 2023 00:56:07 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230703` - linux; arm variant v7

```console
$ docker pull debian@sha256:8e140ce88bd505eebe36c6aebac98f5303b50a067126409f0fc4831ad06b5bc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45124201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e332aa22a3f6fe878a99005e2a42ca5ff1c89e17e08b81d9010ed364042cab74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:01:20 GMT
ADD file:a7c3220804fb0e3fd658c0492b5338ba9fc6c132f28282486bbae9622138fd0e in / 
# Tue, 04 Jul 2023 01:01:21 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:01:31 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:0807315011437359206e59c75af82e26e89ba45ae9281fa33df5e8dda8de17a2`  
		Last Modified: Tue, 04 Jul 2023 01:07:56 GMT  
		Size: 45.1 MB (45123977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c69a5003d0ef8f39c11e33430cc1570553f8fa01a641e6fb1694acb22e771`  
		Last Modified: Tue, 04 Jul 2023 01:08:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental-20230703` - linux; riscv64

```console
$ docker pull debian@sha256:fd8164a7bd9565294d8f433d478adcc1f7371e0ad3431c78beb30d80bbaf2aae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45695712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db54503fa0f89e6f3eee133d4dec5dc6027fdaf9f340fdb7affc4e93354b751`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:32 GMT
ADD file:bacf5c7bb4f9db293679962e5936b1037a72a2e667da59236cda267c866ad8e2 in / 
# Tue, 04 Jul 2023 01:10:34 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:11:21 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:892c64510625aa4b95222221c8d62ebbab44da937d39c14956f6e6697a5c4c80`  
		Last Modified: Tue, 04 Jul 2023 01:13:59 GMT  
		Size: 45.7 MB (45695485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58595682130886a8914b61a3a37dc1da553893a9cf3815062133cff2dfff8ee6`  
		Last Modified: Tue, 04 Jul 2023 01:14:45 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
