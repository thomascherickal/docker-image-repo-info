## `debian:bookworm-backports`

```console
$ docker pull debian@sha256:01b5c5ab0ed3d89cb78ba8a4a1a4c285e47900fa423288fb52094ca2e217812a
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

### `debian:bookworm-backports` - linux; amd64

```console
$ docker pull debian@sha256:d19014ae1dee83e6e83885c7ff2896e30fe7722b03272b6cd10a228db5b42c2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49561805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9381fe4f9748fd7937a47d563243c410d011e72c7b0ed5f0b4e8c757f369df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:15 GMT
ADD file:7d8adf68670e8dc2af6b8603870ea610fc65ecbb08799f2ca6a3134f5d47d289 in / 
# Tue, 19 Dec 2023 01:20:16 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:20:20 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bc0734b949dcdcabe5bfdf0c8b9f44491e0fce04cb10c9c6e76282b9f6abdf01`  
		Last Modified: Tue, 19 Dec 2023 01:24:35 GMT  
		Size: 49.6 MB (49561579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ec03d61deb959613c176bc4628d287e4b831399f2ea20d391b937fa705122b`  
		Last Modified: Tue, 19 Dec 2023 01:24:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:24fd0ea38d6c516ee933965ac0c44c751d93424f81be8bf9c97f9d89e04d2e92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47319463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c23b7596035c16d115229251d3697f353b5b54d5521f7df8ef4a88f8f86fade`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:55:14 GMT
ADD file:a6a83a649ad34de44e3b18ac2ef474733028a38445b36395b37a47906a17e460 in / 
# Tue, 19 Dec 2023 01:55:15 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:55:17 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f3aac8ada11b4cd51c598b397af8986343d5ffa06ce2a7a7c7c80f4ea6f5e522`  
		Last Modified: Tue, 19 Dec 2023 01:58:07 GMT  
		Size: 47.3 MB (47319238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcef8662a50e1cc07595031593533693934fb8d88ca460c241117f4b89ddcad`  
		Last Modified: Tue, 19 Dec 2023 01:58:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:4724dae5f16675e5df66b20445d6d382b7ab1147040600dc50d8155b50a3ab24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45156923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cc80783b1c2e818d022aad81b8cbfd3026403ff5bc675e97fad95a67d5d9c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:07:39 GMT
ADD file:1633615de1824a95e35747f0133e90ab5ddc138574a83fb9c4f337cf45762574 in / 
# Tue, 19 Dec 2023 02:07:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:07:44 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:89cc9e7932dc0f797e6c3fc84b4c6868fedaca1b174b38a51e152a23a643be7a`  
		Last Modified: Tue, 19 Dec 2023 02:11:28 GMT  
		Size: 45.2 MB (45156699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59cb823222f629c853fef9e0f8105a11767651183749cfd6523ea06c9cce589`  
		Last Modified: Tue, 19 Dec 2023 02:11:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:63148e34f2e7f12efe9d3c95a3811439e4ee219be45dc450cbedd3c4f2471e96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49592487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2aef6655592c7369f0eda5b603e9ca26b09ddb2f5e5df3043415168d58b0852b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:02 GMT
ADD file:412f80f75ed3e520f767e70b6b27fc81807f62fc5c6e5adf756507e33af9fa6b in / 
# Tue, 19 Dec 2023 01:41:02 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:41:06 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b66b4ecd3ecfb67b3b7a2a44b0199cbdfc94965c8bd3fefab75cd2e612799740`  
		Last Modified: Tue, 19 Dec 2023 01:44:14 GMT  
		Size: 49.6 MB (49592259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2166b2aee98ec1f3f61b6a986a5751da4a436b6fdb81cbba723d62f34f8418b6`  
		Last Modified: Tue, 19 Dec 2023 01:44:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; 386

```console
$ docker pull debian@sha256:e84198437eb8eb35656378e3c36ce5dfe07f0658511b1f883a7f7bff66163ccc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50582541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47855d4694fc4ea8e8f9da42fd334e169de3dbba3838697f30af8ef0a45e1753`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:38:52 GMT
ADD file:c20aace531a43765f8c1b69c75d7f46a4ab443377a663ab47e0bb2ceb013a611 in / 
# Tue, 19 Dec 2023 01:38:55 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:38:59 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9b51fe964cb335e4bc3b61dca07146c7a0aa4c31e5ae9fec90f2a950818a21a4`  
		Last Modified: Tue, 19 Dec 2023 01:43:18 GMT  
		Size: 50.6 MB (50582312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627f822572fc20d48837c6eef263d589c56ff880aaca326f3627242fca713901`  
		Last Modified: Tue, 19 Dec 2023 01:43:32 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; mips64le

```console
$ docker pull debian@sha256:3a43179cd203dcb836029aa7ed47ca5035d47a24a3aea44401670b708309439f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49549088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f48cce95791a082caa0d1528a05764a4e59ef659d59e2317c868387dce3f40`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 02:12:55 GMT
ADD file:87d7b313e4309f5e9ad824dfd7dc6f9a85458ccb7056f5001dc6066e964eabcb in / 
# Tue, 19 Dec 2023 02:13:00 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 02:13:14 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:659946beb815c8c0157caa0571c5512c4508ff0fe3bbb59e9513e933c7023366`  
		Last Modified: Tue, 19 Dec 2023 02:23:53 GMT  
		Size: 49.5 MB (49548860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f822765ac762672a1c90192cbd4fd444972cd32dfac51be41c2407aa40264f1`  
		Last Modified: Tue, 19 Dec 2023 02:24:09 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:69de9ae71f8286933a319382bc97779c91114d7be072944b37fc3ce68462cc3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53557971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7934c17376b790cede323e66a00734b18b4c85e3dc1d5e4e857fbc0365f9222a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:31 GMT
ADD file:1728d055717ccd4f036c355a84deb6451942dd6e2c7998ee9d9d4edb3c02f7f4 in / 
# Tue, 19 Dec 2023 01:21:34 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:21:42 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:b5382b02d02e48b7676d14a370941b889916302c0c0a4ce6eed6a87ddd65e5a3`  
		Last Modified: Tue, 19 Dec 2023 01:25:50 GMT  
		Size: 53.6 MB (53557744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25ee12c5ca8eed06e698cab17c93a3d6a344d431abc044d467051d6107e2fe`  
		Last Modified: Tue, 19 Dec 2023 01:26:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bookworm-backports` - linux; s390x

```console
$ docker pull debian@sha256:6a23b463fc40e65899c8004572a58aa83ce0e6f4fffcf7a62a4d71f14ed93c93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47917904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e5b33f061b9b6dd7b678cb5057071dc0c47634678411ca41e10ff2a4cb8f64b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:42:12 GMT
ADD file:5e36efc0891837fbd669c10cc5082f41b4ad22190feb2d516f4f0efd4890e772 in / 
# Tue, 19 Dec 2023 01:42:20 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 01:42:28 GMT
RUN echo 'deb http://deb.debian.org/debian bookworm-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9ba06e3db941501f326f297f1b24643ce2b142581fc9f396effcbc7c63df4938`  
		Last Modified: Tue, 19 Dec 2023 01:47:24 GMT  
		Size: 47.9 MB (47917679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8155d26e03c2cb2313e75b0f4187c507223769910c27eec3bd39d8ccd1b79b3`  
		Last Modified: Tue, 19 Dec 2023 01:47:31 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
