## `debian:bullseye-backports`

```console
$ docker pull debian@sha256:44e4d00fe245bc2304b24722937dd3b6a9a8abf7695a52661128c6fac92e58da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull debian@sha256:7fcc614774505fb2653e9239ed899fb97d9102985c4d01d386836dc0337ad859
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54898446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b729e67c136d71b2c26ad3440dab0af1e65a5f671e16b0b70c88022fc793582e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:59 GMT
ADD file:eebf6f761892ad2407885aa93a2abf7647cf0367e3590f3cc7971594ff47193c in / 
# Wed, 23 Jun 2021 00:19:59 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:20:04 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:d28ba3bddf26336a2dff9ce3319ecd166971168469860f171fa659f62cb3ff6d`  
		Last Modified: Wed, 23 Jun 2021 00:24:24 GMT  
		Size: 54.9 MB (54898218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa66b74555e90fa40abad76077ca4a8acbdf9c3fa90c81264483402e116c0a0d`  
		Last Modified: Wed, 23 Jun 2021 00:24:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:f83e6ba0a0a95ab501be17df98f436a0086f2cbec24a3b98ccbd5fa734432f36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52438615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cafe6d4f99fb04a85ce2fd8103fd47acf07b7388003f3a88cb8de86e9f59304f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:48:50 GMT
ADD file:b1ab65bd906b52c44584b6aa35e2e9a14d5fccf907ac8b12a8bd3ab106368f8d in / 
# Tue, 22 Jun 2021 23:48:52 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:49:03 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:935ccf98b4128795cbb17daf7b631ae49bbffbf371e91db72950c1cc501fec30`  
		Last Modified: Tue, 22 Jun 2021 23:59:35 GMT  
		Size: 52.4 MB (52438388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b026661d3ae9c1e2f883a691a26992e4daef752ce010f6953eda8a1cdd6bb7`  
		Last Modified: Tue, 22 Jun 2021 23:59:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:005724ee71d7d70489e6f24c4efffe40fcc74d87b4fa95e1646bfed1ac3915c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50099439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:355663f571e95c2b3fa562bc7ddc4565ea88edd2ae9486a08219e8a77e794fc0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:11 GMT
ADD file:ad79d7d1e72695a6bc5bc7faf963aa10b7640e18d61799368c033154d25f4074 in / 
# Wed, 23 Jun 2021 00:19:13 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:19:24 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0d841baf75fbfb347b67a1e92382bad913e5ece75d2865565bd39c673601fca0`  
		Last Modified: Wed, 23 Jun 2021 00:29:49 GMT  
		Size: 50.1 MB (50099210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8640dcf523934aa3e4ca0ad2c60308748bc335d0d70e0301ab3d6d4e82842a`  
		Last Modified: Wed, 23 Jun 2021 00:30:01 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:650a9e59a49cb140d3f24c031d990d0f33e840b58ce07004a3393db914c1dfe5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53582235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b8eb380668e7239f3c501fdcb65652f3207ab9da5f32a76e3fc1d8abbf7356`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:00 GMT
ADD file:4a6460733f3542d1957e24a1b1640ad7a76b0e4d8aee727e7d2ad9ecb8baa5be in / 
# Tue, 22 Jun 2021 23:49:01 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:49:07 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:764e5bfd58ff2b8baf2ec95af0b179082665955a271e28d9b50d4ff1917c2c0b`  
		Last Modified: Tue, 22 Jun 2021 23:54:07 GMT  
		Size: 53.6 MB (53582009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccaf15d228f28512fed6e72c53aaa475f8ba141fc6dda9175bffac82251494`  
		Last Modified: Tue, 22 Jun 2021 23:54:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; 386

```console
$ docker pull debian@sha256:8c3a9b649c2fbc050fb022f9cffc95ad33ed568cc225183e0e1f7856d0b6d031
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55914604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9317eb2cfe02d61bbeab60238ecffbea0f5ee6bd4058a781c73530b6f6d73c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:38:49 GMT
ADD file:ed43ceae72cd0b1a1ee0ecf4319bf0a9ff0d8cc4542a983609d4df18ccb3133e in / 
# Tue, 22 Jun 2021 23:38:50 GMT
CMD ["bash"]
# Tue, 22 Jun 2021 23:38:56 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1a1a10c368f246da8fdeabb7eecba4e66e58cdc28feb3b3f7714896e4f52dd56`  
		Last Modified: Tue, 22 Jun 2021 23:44:57 GMT  
		Size: 55.9 MB (55914378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9121e475c318ba593ab815a40496498cc0364d58fe0c59ec36e29891d192825b`  
		Last Modified: Tue, 22 Jun 2021 23:45:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; mips64le

```console
$ docker pull debian@sha256:dbc6c158c8507e04eaa2b0dc8d74fb5f89e22c5ece7b68500d5c924270aa35f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53153194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5644aedc94f9d764351f833f3623753e495ff5bc2f7d0fd36d38b85d11c8acef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:08:19 GMT
ADD file:c35f12783d634fefd92f2d45605502f97a497b66a15f60dfccb4b2a2d4a293cd in / 
# Wed, 23 Jun 2021 00:08:20 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:08:25 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:3ebc6252e914164fc2a31f5418122631ab0e70c83ecb8f8b24f7e1ca5f4f2fa1`  
		Last Modified: Wed, 23 Jun 2021 00:13:48 GMT  
		Size: 53.2 MB (53152965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6177c28a275d98a2c98787e3146395eb099379ec9cdd41d8f7062308e1100712`  
		Last Modified: Wed, 23 Jun 2021 00:13:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:435b66bb1dcf535baa53c1a2836a7ae12ec9f40b7d65d711156b742b03d73893
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.8 MB (58811100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a28be79602fe84e7d7d58ebd7ad6fa9df09dbf679bf0c36a8c86c005e9ae0caa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:28:56 GMT
ADD file:902a353e8fdec64f149d504baaf70654faec8f23749856644d0edeaf32da0fba in / 
# Wed, 23 Jun 2021 00:29:08 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:29:36 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:09c77b0cc13f990901884e4cf084070a3b7c2d5058b18159ca0117900336d82f`  
		Last Modified: Wed, 23 Jun 2021 00:35:48 GMT  
		Size: 58.8 MB (58810873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4a1a26102c5a2de178c25e064ec660fa66c7a1775daeef5af3a0e882b9ff7b`  
		Last Modified: Wed, 23 Jun 2021 00:36:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:bullseye-backports` - linux; s390x

```console
$ docker pull debian@sha256:f44e3f195495c130d1828b2c6ce93c64422ddff3950d4978d235d6c233a630df
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53183452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59ae9682a1426f5677e812258cb3ea9eff9589f2673cc9f6570048264474df2b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:49:41 GMT
ADD file:c4e658e7b0a2f1bcd1adbc3f8d4b90c39d22edd3817e41078cce53daa39778f0 in / 
# Fri, 09 Jul 2021 02:49:42 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 02:49:50 GMT
RUN echo 'deb http://deb.debian.org/debian bullseye-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:616c5ebef764d038df48c869a270b4c696a19212343d41c89f2f771e65bc2219`  
		Last Modified: Tue, 22 Jun 2021 23:45:00 GMT  
		Size: 53.2 MB (53183223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2acd3f0e0fd7e4cef3eba2c743a83c0f629115b84176a612f8669fac73b8623`  
		Last Modified: Fri, 09 Jul 2021 02:54:26 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
