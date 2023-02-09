## `debian:testing-backports`

```console
$ docker pull debian@sha256:0ae409e840eaafa52a60ab4656b7700e76c2fc331d93c53daf117a2edd8790d8
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

### `debian:testing-backports` - linux; amd64

```console
$ docker pull debian@sha256:e1aed714f45d53c09dcc609f0d8df974976a5a353c85a48a0da45ad2268f2169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49055144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d91560b15b23dffecfdf11c7a808fc80d118d44b512252aacbc3c7565742bf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:22:23 GMT
ADD file:61fa43fa946b222761867772cda761bd169bbf7db3ae93f9f76a0ad5e23a1c31 in / 
# Thu, 09 Feb 2023 03:22:23 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 03:22:27 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4bf9c1a4a408851360f1c5240bf00f9a9ef6c81b3c141c0a059cf86fa507c91f`  
		Last Modified: Thu, 09 Feb 2023 03:27:48 GMT  
		Size: 49.1 MB (49054921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f02dbb32fc0e6dc7d101de2af3b2229578916b043dbf25737fb572bb613f5fa`  
		Last Modified: Thu, 09 Feb 2023 03:27:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:bc2b75add89c6f75a77c68e51988e3e68fb9bb82c94cfb49181918d2594fa8e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47988984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdd6f2d877713bd0d8f1c45eb6e4bed735188c0ae61f71817212fb5fb97e0470`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:01:35 GMT
ADD file:cc1f667d0ba4529e861b2055eda82a740a2518ccf9366dc1cb94dab2b6c1e1b2 in / 
# Thu, 09 Feb 2023 02:01:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:01:42 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:952d0258fb8c640f2a3061d2f287d2075d603b7608f8d567d117c04bda5478dc`  
		Last Modified: Thu, 09 Feb 2023 02:07:26 GMT  
		Size: 48.0 MB (47988763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeccfed158aa4af8e8025f6aeb9d71f589d0691c1e9f97b0bfe1d699943ed36`  
		Last Modified: Thu, 09 Feb 2023 02:07:37 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:29f598bbe94f6e034e46ebde69e3e34e0e931cf823799d39c9003b04bbd34006
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45794386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5f5e81ef4843f17510606fbd2e976af3968276758fd0785d66216fb34303d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 10:01:46 GMT
ADD file:0a9c474422e8c0f119b0473bd550098fa14ececd6f4e1ebecb0519057ee3949c in / 
# Sat, 04 Feb 2023 10:01:47 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:01:53 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4acd2d529567dfe96a5a0e4495609a52502ee02aa4ee77b1c33f6157e5f09282`  
		Last Modified: Sat, 04 Feb 2023 10:09:37 GMT  
		Size: 45.8 MB (45794161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad901c40241e7172194a257a7e1243d004fb4aabf530377824687aecb68863e3`  
		Last Modified: Sat, 04 Feb 2023 10:09:48 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:e679509f8b3b0f0e6d580b65a6281cb8c622e9e00c8db1d9fd5d532a6a0c3036
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49106003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31eed13984c9b3140f0d9510df12fa76e237d0420dfbe69134161057ebf2abc2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 04:00:03 GMT
ADD file:45b2a619bf39c393041387f1e1bc57c120715c388548d3b19d7c6a57be833081 in / 
# Thu, 09 Feb 2023 04:00:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 04:00:07 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:79154c96892a78a74ca3e3ffa99c5d47ce44f57543cec39875aa7d168c21a18f`  
		Last Modified: Thu, 09 Feb 2023 04:05:01 GMT  
		Size: 49.1 MB (49105781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3229f9e5409a8b53957a62b3b978c45d0c0dace32303fc7a68522dd0d5ab3a3c`  
		Last Modified: Thu, 09 Feb 2023 04:05:11 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:4f8887f629002e963ec510c8b1ed08392464dde3bb09448ee448e44f61fc4931
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50093648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d63cde2419dd8434c5743e075934069eec42b3eebed67bf173ba32f0c518e346`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:51:12 GMT
ADD file:ad17cd9a85b389575f6b3289675831e1173edaf33986260823441a61f1c904ce in / 
# Sat, 04 Feb 2023 07:51:13 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:51:18 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:661528ae13ac034793f44e59402c02c52f6728f6df010da9e53b93360a821eb8`  
		Last Modified: Sat, 04 Feb 2023 07:58:02 GMT  
		Size: 50.1 MB (50093425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3fafc776e44bfcb3358bd3606e29200dfd77a4154935206a369d0466d7ad69`  
		Last Modified: Sat, 04 Feb 2023 07:58:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:28a3a172db437a3ba050609a6dfaa609fb52e7677c5db00fa16dad9b1d3281a1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49063716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e75d67a6620f4e3bd24af72a6519de6956a9a0c334ef5231a8347980c37c151`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:48:25 GMT
ADD file:337b4d04216e44b5e0cf9ff9b037306a185c46f53258a37ccf754947cb4f3b15 in / 
# Thu, 09 Feb 2023 02:48:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:48:39 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:4e42f0862e6c861d6806da345a484c79e45715afe9f8b2e30f6fbe08ddb16e19`  
		Last Modified: Thu, 09 Feb 2023 02:56:57 GMT  
		Size: 49.1 MB (49063492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e239db23d135d730ac49f89bec1c6053d59ceca6bc1c016e77134933f0b61644`  
		Last Modified: Thu, 09 Feb 2023 02:57:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:798e279ae4790690ad545242f2831de9ea3482cced1a2ad3bf77d714504eab8d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53066789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9d9e1f3d32726a50c6679337155203854705bcf1d31170c7a90e2592e8e529a`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:27:38 GMT
ADD file:6a8cc39d059a87a9be2271282490dff13195c22926b3dd5458cd80a387fe6f53 in / 
# Sat, 04 Feb 2023 12:27:40 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:27:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:62e04a70589e68af436acb6cbbc46421df8df67fd86623b045e1f16d4b3c285a`  
		Last Modified: Sat, 04 Feb 2023 12:34:14 GMT  
		Size: 53.1 MB (53066566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1e27f8bdd0ef89d5a0a53d06cc7b41b17f4eea83cec5eff63f277e9a797a8a`  
		Last Modified: Sat, 04 Feb 2023 12:34:25 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; s390x

```console
$ docker pull debian@sha256:279d486458c4c433f36c4dae86a8674edc24d2dad113213d06c1e0dccd704c01
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47428790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d0703028263a66a436462126beba4f744bc2936ae1b0e2f40f83b67f6d6fbb6`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:42:50 GMT
ADD file:60cb89c35b3710b0f052b4bafc231a70af5da7d1bbab581b2e0c88c784e1f08b in / 
# Thu, 09 Feb 2023 02:42:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:42:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d678278d86c767f56825e572ccfed0f53cace096562b0126c42c45b5b2016cfc`  
		Last Modified: Thu, 09 Feb 2023 02:47:15 GMT  
		Size: 47.4 MB (47428568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee963dc7819c5e32e62c2474ba757284dc2b118053b85be86b8a2860b7f25754`  
		Last Modified: Thu, 09 Feb 2023 02:47:22 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
