## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:57bc627e42b4c7b16b3c7a2179946502c4942cd631170c41eb8ae333a0c0c7ad
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

### `debian:bullseye-backports` - linux; amd64

```console
$ docker pull debian@sha256:f6714b86161d1aed4e4d33b82be30a890e856725c404ad473b32a3cdb6e1135b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55041566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5469bc2a392ab2540b73bce3d37260859a265987ae4d88e99410a8eee3e0eba9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:41 GMT
ADD file:553d20b03d45305e58cde07e0c259421bba044155ac90b4559e5cc0b69093347 in / 
# Tue, 06 Dec 2022 01:20:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:20:45 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:f2f58072e9ed1aa1b0143341c5ee83815c00ce47548309fa240155067ab0e698`  
		Last Modified: Tue, 06 Dec 2022 01:24:48 GMT  
		Size: 55.0 MB (55041342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf5828a979d902a48febc8177aacc67a79ba8120aacae287bea852baced560f`  
		Last Modified: Tue, 06 Dec 2022 01:25:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:d8719807b093df3ec60363113b4930b84f668cf9ecd87f1b7f56cef5281827d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52545023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9058567953d44f0a695a2c448fb6a23ca360139e687716a86c1c21c7be67b7c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:07 GMT
ADD file:92bc802977fb4abf65d3a11a702509aece192d088d815bf79a0e6bdb5a8b57c8 in / 
# Tue, 06 Dec 2022 01:49:08 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:49:17 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0eeca4d47a0d9a966ac355f8eb8d728ca02c90f2db97fac6164fb9dd7eee639f`  
		Last Modified: Tue, 06 Dec 2022 01:54:02 GMT  
		Size: 52.5 MB (52544799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f61db4b316b9644e5a64ea5198997d338ffe2750468bfa0ee668470aba88c2`  
		Last Modified: Tue, 06 Dec 2022 01:54:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:797f3584d9ec626697449ecd80ac1e69a2d3c01a54b5814e2174fbd0db3f8f88
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50207313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c04a8b8754e8218b2c637773a13fb06218e0f4668bbb6853ac1a80f19b6b86e0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:30 GMT
ADD file:72eaf12ec65c98e9cde1654b6adb2b3d19f7d81c13b12801c198f699252b7503 in / 
# Tue, 06 Dec 2022 00:58:31 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 00:58:40 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:58e27900c24f1f8f5b6b5eacbc073583f2372b58e9f5678dfe171b496b9cd71e`  
		Last Modified: Tue, 06 Dec 2022 01:05:33 GMT  
		Size: 50.2 MB (50207085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7c2b05534a97f44daa31087ab617829c0cdd24887dad490c696fdbaa01474b`  
		Last Modified: Tue, 06 Dec 2022 01:05:54 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:2ecc623d8ecdcdb8f5713f832fb6426e5df8a632454fa86efc4b86b75f9e0bd3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53699370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b4ed82197fc3738498ed3cc5285402e1d17d636cf13cd6d1ccf83384fa100b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:06 GMT
ADD file:b1e7652678bbfc9556636e77d79c947ff1436888e2929f9c5c3ddb42a50c1176 in / 
# Tue, 06 Dec 2022 01:40:07 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:40:10 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4948a51a9a3f176f30ac619014f4a2da453a943244eacb53096ee9742eb7cef1`  
		Last Modified: Tue, 06 Dec 2022 01:43:33 GMT  
		Size: 53.7 MB (53699146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2ba695ee23c89a841ece02d1afbc99cd343ed9f8082d532b2b6f8677da0e53`  
		Last Modified: Tue, 06 Dec 2022 01:43:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:6f3ad8d925313326afcfc880ec469cafb5092f41d94c07f89a91fb30ec1d6a8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56022611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7d896b5a11eb39c3e3f75354f54380cbef66e67e8c6cf0e8ff6dd92cf930ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:34 GMT
ADD file:f84226ae95254e2a6a67086b709477f04fcf4d6c3a6ed05dd9cabcda0156ec04 in / 
# Tue, 06 Dec 2022 01:39:35 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:39:42 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a9be27fc8e6e19a1a3d5f3a8805c7b1a4c21e2db96b34ed6fd26bb06b286b67f`  
		Last Modified: Tue, 06 Dec 2022 01:45:14 GMT  
		Size: 56.0 MB (56022389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2019581186642596ab1660223f78267eb5c87deac607247851bf0132004eb0`  
		Last Modified: Tue, 06 Dec 2022 01:45:31 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:8dcfebdb2e3932fc38647cb85fb3480ed15b6a34145275727efe59626e5da8e4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53260857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dd1e550c22a8060a056e55baf46b34bb65882d091ac4ab87977d3fcbfce3b58`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:54:55 GMT
ADD file:09d48994a41c54566f7123db033773e6246c0703a518af76843198196cd39645 in / 
# Tue, 06 Dec 2022 01:55:00 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:55:09 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:acb57a81743c28ead1a32571c107ac15cd970593fea4f2954b57f22e6bbad1d0`  
		Last Modified: Tue, 06 Dec 2022 02:02:59 GMT  
		Size: 53.3 MB (53260631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac02f00f42a102dc4f5fab5d3f6c7d26f895509ee76fc848255077a4c2b019d6`  
		Last Modified: Tue, 06 Dec 2022 02:03:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:b54d16d026045414e22e9c1d9ec064d385544866b820db0f70bb41eb4951be10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58913361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91bc30eeb0bcdc30d4e778538ffb7ce4c45ace1b98eeea9a9fc54fd7448cbcea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:17:38 GMT
ADD file:1a9427ec1dc5ca60bb760d16d5d76760f730c0c0eda8382a1d28a5e50535ad7a in / 
# Tue, 06 Dec 2022 01:17:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:17:49 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ff7c811b7837034ee1579672c45bccdf29d765e735d05c933d69b7a21769ff65`  
		Last Modified: Tue, 06 Dec 2022 01:23:42 GMT  
		Size: 58.9 MB (58913134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368ffc71bd73feed1556bc836fad1a05d383a37c6772ccd02b50e5ceb02e08d4`  
		Last Modified: Tue, 06 Dec 2022 01:24:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:ff38718dba116058790b11b6b64cbf1ba340de4b720ee8211ed4717db35cfcf0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53273111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea82e477637d626d7d6f9bd243b5d4bab172863d0083ffd3865361cf8b70a75f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:42:37 GMT
ADD file:022ca98bcf37301887c0e5d24eebe36e6c81a037e13434cf887bb848aaabe291 in / 
# Tue, 06 Dec 2022 01:42:41 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:42:51 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:a3a57c761295cdc2f327925c14939b8b76fff91be8573eef2420cd05dcb39c1c`  
		Last Modified: Tue, 06 Dec 2022 01:48:26 GMT  
		Size: 53.3 MB (53272886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9205efa7b7bde8b893738af9297750318e2f2e00a011f9beebecb36b96b299`  
		Last Modified: Tue, 06 Dec 2022 01:48:38 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
