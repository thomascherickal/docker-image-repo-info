## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:b49ccdb0ab5bc35b0b622e395282edcf9ea0e0b52769ce7435d02bcc52ca0f10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:51092cbec226f662a97ab8f224f1c6a22c784015b39ebbc06812a0828a22b0ae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137682711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86552ccbf7feeef5f1324e901fcc4b77049d31af9ced94638b9fbd1fe3fa7fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:19:36 GMT
ADD file:aea4560c39a3a877086fc63afdf218ba3600a05abef7c44563f788e8b60c04ef in / 
# Tue, 23 May 2023 01:19:37 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:45:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:45:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c98dda1b0e97e7fa61fa33cea43f85bb1a36a4f6f65c7b8430cae442b76ece09`  
		Last Modified: Tue, 23 May 2023 01:23:14 GMT  
		Size: 49.3 MB (49301275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a463ac54ed3eeee295443fb87b28643b95d7975e83bd214bc93db462b1b59de`  
		Last Modified: Tue, 23 May 2023 01:55:08 GMT  
		Size: 24.3 MB (24274092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7076663891554c4b6516ec84fd2d5459502966e94b4d794796b086aea4f4ca2`  
		Last Modified: Tue, 23 May 2023 01:55:24 GMT  
		Size: 64.1 MB (64107344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e47b720b35ad887b644c94481713f1d2aeab7646224b6b5084d767cea5479613
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131671128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe93bb920dac94f750d11119c6fb44d3e36fe4979b953b01468151f735a7bb4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:48:16 GMT
ADD file:8fc8e3b90ac0435374d713c6b80b23f1db0866a447cf839ea8304d4717982da3 in / 
# Tue, 23 May 2023 00:48:17 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd47f968dbd1b839925549bb9a90d021c19486875443123fb77e8cb1367e9745`  
		Last Modified: Tue, 23 May 2023 00:50:22 GMT  
		Size: 47.2 MB (47168971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58dcd7a31d73fae7c8f3da6415b83f56c0b8c1635526741fd0c65632ae15973b`  
		Last Modified: Tue, 23 May 2023 01:20:37 GMT  
		Size: 23.0 MB (22950966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64527cb5109ec935f8bef268d9948c57924a7b5d1bbcda29e980f1bf4a6a37f2`  
		Last Modified: Tue, 23 May 2023 01:20:56 GMT  
		Size: 61.6 MB (61551191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:331db16e2b01d1927b127fda6bee4baaf1afe723687ad2f28537e9ccccdf534a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126423598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd030fb412ac7e3dd0bb5fdab07c73d829d6a214545a719a34f87de4e32bf5e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:57:23 GMT
ADD file:76738dad56d76cef0c57f5c574260e6494d397ba6ea95f5ea14ceeda292e8a0d in / 
# Tue, 23 May 2023 00:57:23 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:51:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 09:51:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b62ba7ac5fd70caec3910c292af59431036e6a2f6a4fc4266b3c04d3f6f7febd`  
		Last Modified: Tue, 23 May 2023 01:00:49 GMT  
		Size: 45.0 MB (44989913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5316b360a91afe489f52f8edacb51535faca57922a648164ceab10593e7842`  
		Last Modified: Tue, 23 May 2023 10:03:35 GMT  
		Size: 22.2 MB (22176633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d1443969900c81509f08727255738a226e326b2e78357a9f564ed1a40e0de`  
		Last Modified: Tue, 23 May 2023 10:03:56 GMT  
		Size: 59.3 MB (59257052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bda807282d57ca94acc2800799db06a6c9055a150d661239e169e3641793c8ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137143007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d32be9f731a49a7943f690105493ce19ef9e608d296754dfd7d5df786d737233`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:54 GMT
ADD file:91184714f613e1768e87fad722350f471376a88cb595664e8e23864ce5d79071 in / 
# Tue, 23 May 2023 00:42:55 GMT
CMD ["bash"]
# Tue, 23 May 2023 05:52:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 05:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3485dc61c38c6db2e8092e9f4326fe6c51e867a1841f55346f74ec25847d7401`  
		Last Modified: Tue, 23 May 2023 00:45:14 GMT  
		Size: 49.3 MB (49347785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f929165e3c93f5d762267d93e97574e2fd7ebf4c98f33a2664ca58afb970b9a`  
		Last Modified: Tue, 23 May 2023 06:02:01 GMT  
		Size: 23.8 MB (23810063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cce032e95f3ca3e3210588e183ef0e95a0ab610151c718bf68d1f7f497f4a9`  
		Last Modified: Tue, 23 May 2023 06:02:17 GMT  
		Size: 64.0 MB (63985159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7285ecb58abaacd425e46a8f49f8848527e92124aca75931d3946c1485e6553f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141403547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829e40641db120e27b6767c9d5834e7a3fa2066af32effc700c78a83725e9393`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:38:43 GMT
ADD file:4d14207b5cf935fa2b9de70132f41a0eb90a8b5200ed3d27e60b766fc6131e13 in / 
# Tue, 23 May 2023 00:38:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:54:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22e40771358829b6817b47cb2d682b51257385478c18bb1ec96251a68a9c75e4`  
		Last Modified: Tue, 23 May 2023 00:43:23 GMT  
		Size: 50.3 MB (50323189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bf109a603c637e9a80a5a8fe46353089a5fb8c6333eced350af89d7298576`  
		Last Modified: Tue, 23 May 2023 02:03:46 GMT  
		Size: 25.1 MB (25110482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39204aa4c310e5b428093f5182d87e2f302dabb686c85507aed2372505156242`  
		Last Modified: Tue, 23 May 2023 02:04:08 GMT  
		Size: 66.0 MB (65969876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a28e3e52d5e8501460ad0f433ddd327754cef7c299876082bf8ceee5d0ecda35
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136117227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5261b221a9ad12c69fa02f279869a63b04bdd93b9fbf19edfcddac08408b9de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:07:59 GMT
ADD file:c8965d5e1a440e4bc93318be2f80c95e9692ada237122031d2e98793b8036143 in / 
# Tue, 23 May 2023 01:08:06 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:42:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65775e721f6c7f76e54f65c03408a249103c86c536e6a86498f9f5a6229b9f4e`  
		Last Modified: Tue, 23 May 2023 01:17:24 GMT  
		Size: 49.3 MB (49304239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464924f070f4f4c8a4e8facea0026336e200a0c517951d62854dc3b3a1154f58`  
		Last Modified: Tue, 23 May 2023 02:06:54 GMT  
		Size: 23.9 MB (23864351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359f2eaa37862504aa49ac76cb23ed1f915f986e4579bc54affd5a7e8ab8f277`  
		Last Modified: Tue, 23 May 2023 02:07:44 GMT  
		Size: 62.9 MB (62948637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a70fee0093fc78a9ced3f519cb0f01aee68baedc6ac1f6a1afa1cc11103d3ff1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148803187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e212d4fafe68f0c10626374ccb6d62ba1b8d22f76d5b5913300ed6cfe2ba0c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 01:16:38 GMT
ADD file:28e774b3554d274fc742feac48f78a3bf6f120cb729e2824007dd94d5c414156 in / 
# Tue, 23 May 2023 01:16:40 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:45:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:46:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e109feef3fc6307cd9a880958cef6624de9c2c6f054987e479461a1ae51c7503`  
		Last Modified: Tue, 23 May 2023 01:20:49 GMT  
		Size: 53.3 MB (53312324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab84a55cc084469df8b38ab6a01658bfba2b29b7410a970ba6d9d2864846672`  
		Last Modified: Tue, 23 May 2023 01:59:19 GMT  
		Size: 25.9 MB (25923867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfbe0bc6dc85168e7da83a7be20c9913921338417e0c639a93ff1cdc5664403`  
		Last Modified: Tue, 23 May 2023 01:59:46 GMT  
		Size: 69.6 MB (69566996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9e1d58d54da9f531f48f7da4e9eb1ef172f8abfd60275d5e7833ff3b286c5d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135054673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3c11d4a07fc41d0ed681756a03518e460b192440f51d9e10acefb26e3bfdd50`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 May 2023 00:42:04 GMT
ADD file:cc95a0712a6bccebd449eb4ff979eeed054299ca9b7766e545c76d0c23c957ee in / 
# Tue, 23 May 2023 00:42:12 GMT
CMD ["bash"]
# Tue, 23 May 2023 02:31:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 02:32:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ffb123da88ae28227159c41b0f21826f6497089ece0b790a5c14d890cf50771`  
		Last Modified: Tue, 23 May 2023 00:45:12 GMT  
		Size: 47.7 MB (47673474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3541e04aeeb82d496c085951f9619fcdf7bce92b4b7185f684cbb7ef6f65ea32`  
		Last Modified: Tue, 23 May 2023 02:37:57 GMT  
		Size: 24.3 MB (24270889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b984494917df72746bed1d04a989f9f1cf3cbeeef990a9d0a58690373ab6ffaf`  
		Last Modified: Tue, 23 May 2023 02:38:13 GMT  
		Size: 63.1 MB (63110310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
