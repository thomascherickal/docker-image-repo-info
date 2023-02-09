## `debian:testing-backports`

```console
$ docker pull debian@sha256:46af8b8bbbdc30640b5cf930b853bd0e39d79808794c729030261e2aca2d33b7
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
$ docker pull debian@sha256:cf5bb2cce897dbca412216aa0570e4faa6f8c4014d19dc325972ae730ed372a5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45796074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf5502c67ebdca2f55cee0e8554843f3349bfdde89a196b0d66b5f56752484e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:14:35 GMT
ADD file:bcccad1d9520abd65309399487f74598512fa9c3f8ae0b96de065dddd7939799 in / 
# Thu, 09 Feb 2023 06:14:37 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:14:43 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:7087f0f1cf54a3867b19328991ae19b55c16f8410c5f93797e4e5aafce80db61`  
		Last Modified: Thu, 09 Feb 2023 06:22:29 GMT  
		Size: 45.8 MB (45795852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e8ff4564a604aafc522168b2dab516ea0bc9758c04187c8ea7df332b251030`  
		Last Modified: Thu, 09 Feb 2023 06:22:40 GMT  
		Size: 222.0 B  
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
$ docker pull debian@sha256:1b1b9802b6c84da72c20bfda925393dcf563056edb78a011d9abcd325816c1dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50089622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705078c3debc205764261b6875dd6c8a3093f67b4c8c5a95fcdd0b133836f35e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:51 GMT
ADD file:c163ffc018e92e2c9496cc996695dbd1394ce03e4f1fc531ca164f827090de31 in / 
# Thu, 09 Feb 2023 05:14:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:14:59 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:af8b5355c1334243aa59341c331be504814132619c825bc68463cf631f18bd7c`  
		Last Modified: Thu, 09 Feb 2023 05:21:40 GMT  
		Size: 50.1 MB (50089399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32d591c8d5834f197208fde567ea1a2165086f3a197619f0c1b5179a52a32e`  
		Last Modified: Thu, 09 Feb 2023 05:21:50 GMT  
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
$ docker pull debian@sha256:fb42db36978788c5e8d971aa006afc4e24bdf13487d2488183d2eb0cc7aae27b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9e022b1692278bf92e2a844cfeb90c8b7543dca1f4433288fada15f855a872`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:23:49 GMT
ADD file:c7057d18ca4a344e68cd4336003381471c73bfa31180038a7dda8e515527a203 in / 
# Thu, 09 Feb 2023 06:23:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:23:58 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0054b217e37245df6e913680e7453251097c709a163b68d37e9d06cbfa9d0fb9`  
		Last Modified: Thu, 09 Feb 2023 06:30:31 GMT  
		Size: 53.1 MB (53065009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ce60d54f143c15bdb7d86475f5f8317fd341277c1fd0da8431b6ba16f87de9`  
		Last Modified: Thu, 09 Feb 2023 06:30:43 GMT  
		Size: 225.0 B  
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
