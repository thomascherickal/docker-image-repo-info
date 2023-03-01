## `debian:testing-backports`

```console
$ docker pull debian@sha256:6d1183831394b968802ffb5a8e836e4d42938a1bfa0f9aff5e4bd1dad4d572f1
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
$ docker pull debian@sha256:e8292f26ce78a896ae0c64fa23eefb753aa26c8a8b463aecbdcdaf01eba1734f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48073055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2334c7148c1590a9b2ede897e9ebb66510fa827a27bb86dac9d7abd4de8bc712`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:49:34 GMT
ADD file:2754fb0733bf053663be45fdf8749e4c88158b9b85a85403f9898c3dfb53215e in / 
# Wed, 01 Mar 2023 01:49:34 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:49:38 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ec0704dfd86e01503ca7c8e58baaa3616684e2a382e2ae7ce46e3466830b2a1`  
		Last Modified: Wed, 01 Mar 2023 01:54:34 GMT  
		Size: 48.1 MB (48072831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2df0b944c64529f9142b7c44697dbabf1ad89eb38cbf101f8e7cf9c9f631e4d`  
		Last Modified: Wed, 01 Mar 2023 01:54:44 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:a5c72bc480858008dce9e53be8987f2d867128717b34ca294b588dfcaeb96cca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45843511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef051962bd26553fbb717394fa6cbdd2fc88fce82d45c6290a15dd0a6c4911e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:59:11 GMT
ADD file:6820e6909f34bd7d88f849318c289d08246870bf48e194c42cbb0d2bfe92716d in / 
# Wed, 01 Mar 2023 01:59:11 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:59:16 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:26dc867e29a6399aa4a7d729a815dfe65dea3873cc63f402795055187cb4b88e`  
		Last Modified: Wed, 01 Mar 2023 02:06:03 GMT  
		Size: 45.8 MB (45843289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068607b3ca26ba811ce31d196a7341ea0ea63e14b171b5bcf9d2e0073fa18fbd`  
		Last Modified: Wed, 01 Mar 2023 02:06:13 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:f3ca69490223e830099bfb2ff3762876cdd274971ff92fdae6f3d0781154537a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49274174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:400ca32e84754d40369be03dbad1801a376e0d16def856baba61d9db50ae90ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:21:51 GMT
ADD file:c47730325f9bfe6686c928d0c7c46f6bd75a614ac9bb8bdffdcfef69b5cab2ff in / 
# Wed, 01 Mar 2023 02:21:51 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:21:54 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:bd5a6f14a1228f25359ec5248195de6f015069b0c74dc6be8e415fc08ed74f38`  
		Last Modified: Wed, 01 Mar 2023 02:26:44 GMT  
		Size: 49.3 MB (49273951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34f82c07f7384068883b273ee1740f2d68d4c1256cebdacecaef1a34e646bc3`  
		Last Modified: Wed, 01 Mar 2023 02:26:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; 386

```console
$ docker pull debian@sha256:b93391bc3f9f9c34d0c178f0b6d61424a42a686597469f89e6b8df11b1dcdaed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50273616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8d244b2c2aa266070aee2c27912e0c1ef882553838465763805cec5407cc2aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 01:40:43 GMT
ADD file:c00d2713c83099ce3b5f05e27bf4f23d8f3d1234d35e526c414ad2a77fb2fe30 in / 
# Wed, 01 Mar 2023 01:40:43 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 01:40:48 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:8026e865d4c7ec94ce5b33cfaad678239d3b21bb7b731be6e9adf74ed7eeef15`  
		Last Modified: Wed, 01 Mar 2023 01:48:02 GMT  
		Size: 50.3 MB (50273391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5311deae15dc2300ca2d470b7624df4e6b9266b1e37b4173fd0dd88565877a1`  
		Last Modified: Wed, 01 Mar 2023 01:48:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:testing-backports` - linux; mips64le

```console
$ docker pull debian@sha256:10b6f73020588e97b4d6c35f65cbf479b1ab5110265e79e34fa80c2cb4f0416e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49245732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16940537906a118a74e5b233a78dbf1ccfb92383fafe7e6d9b7ba52d9d64f8aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:13:45 GMT
ADD file:1bf792d3c4330d4faf867dfb2e9689482bcfd0a8d9c641abd7cca9b6a218978f in / 
# Wed, 01 Mar 2023 02:13:50 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:14:01 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:9abd347c7d1810d25b14d496d1aea23dffa3a1bdfd637405ff33a4f90244ddcc`  
		Last Modified: Wed, 01 Mar 2023 02:21:51 GMT  
		Size: 49.2 MB (49245506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1df3a413749712800dd37603aeba16f017976baed61398f73e1f2a83ce6ef8`  
		Last Modified: Wed, 01 Mar 2023 02:22:02 GMT  
		Size: 226.0 B  
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
$ docker pull debian@sha256:d6ce6feae0b90783e1dc5248c5e6c7864794cf1f5bd9270d3b7a33a2fa661eb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47608261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f8ddfd9c5afd4c174f7b8543a1a4f2ce473f730213ba8bc08d38a529d33ec32`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Mar 2023 02:51:38 GMT
ADD file:8439a18edae9de92ebeb6ca0b69fbd74a02cc73bd2ca22601f8258fa87e9d69a in / 
# Wed, 01 Mar 2023 02:51:41 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:51:47 GMT
RUN echo 'deb http://deb.debian.org/debian testing-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:5cd18bb803f30053fbd73f7ae3e9f9955611d476d1cc5d8cd575f473f69eb5d3`  
		Last Modified: Wed, 01 Mar 2023 02:55:53 GMT  
		Size: 47.6 MB (47608038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d828400eff381b7fcbe109a64a73ef1a211c3a20843699322fddde6f341dcf`  
		Last Modified: Wed, 01 Mar 2023 02:56:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
