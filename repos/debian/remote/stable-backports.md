## `debian:stable-backports`

```console
$ docker pull debian@sha256:4c0f209e8c9824f973d4170f9a4e0d34c3b01cd5163ba808ae95cd8aa71a7a88
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

### `debian:stable-backports` - linux; amd64

```console
$ docker pull debian@sha256:bf6b145efa1b559a15fb773c36016cfed6239d0a95f01d6c017d23f47260becc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49582256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b9ed9cd55289e485f8f5f6291bcb428a03f1fa8616d94e751db1836f2ee64aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:47 GMT
ADD file:e4b5d0e7045f4d28d34e728d72d11e967751a1854c3b9e60811be54b1cfb2db4 in / 
# Wed, 01 Nov 2023 00:22:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:22:51 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:ad1295602a0fc01fa0c6a8477bea89b63e96d9a707a9ac8c72a41bc2ac640f75`  
		Last Modified: Wed, 01 Nov 2023 00:28:57 GMT  
		Size: 49.6 MB (49582033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201b6d6593829ec85e8b919775594f3d66efba02128a3bcbf8e0621318a3d15`  
		Last Modified: Wed, 01 Nov 2023 00:29:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v5

```console
$ docker pull debian@sha256:3f96dc95967f40311dfd2066c4049b7b24bf507a7768bade31b1baabded04c0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47355973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e18e52588bdf88d507c8e82431ab7f6611210056168917dc32f301860f7a14c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:48 GMT
ADD file:05d4f483ed515dc47d5bd1f7e5e90bc3d02821818848c5b00f52d37f6f7bff4e in / 
# Tue, 21 Nov 2023 05:01:49 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:01:52 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:6e02f47df7e9ddc4b1f964075a0833af0f7a97a67f6ce871d216de797408d47d`  
		Last Modified: Tue, 21 Nov 2023 05:06:06 GMT  
		Size: 47.4 MB (47355754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4799997a13f7946213c2709836ccc392f10f18e31f8a210001580172f37e5358`  
		Last Modified: Tue, 21 Nov 2023 05:06:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm variant v7

```console
$ docker pull debian@sha256:753de1e18aafaf319a010ee1aeb33c919fb550aaaea4f64f1a8b5e95450021a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45180275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e0373d77b1984bc765ce8c6f80a295e6fd23a4043128e8c4ab0a420b35b00`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:59:21 GMT
ADD file:9449e70119877a15c4e32fd928c3c66d5ef3bceb73ea3ea9f42a9d37c35114b9 in / 
# Tue, 21 Nov 2023 03:59:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 03:59:25 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:0681e3a8af101f8eacf74d0544d2d3870674cfb10dea2824fb7a397fcd472bc4`  
		Last Modified: Tue, 21 Nov 2023 04:05:24 GMT  
		Size: 45.2 MB (45180053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8d0fca79629165459821f8238ec1fe4ae3a1172c424e876e413a7e5133ad3c`  
		Last Modified: Tue, 21 Nov 2023 04:05:33 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:b270c7efa4ab105fbe5b7071b66f65f2d5e3543815e7a01e40faa3021c864c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49612880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6de2dbc256ac9b29f48a722b13207a3b44e6029abf521066783a24ddf1005f1f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:57 GMT
ADD file:5ae606dfe6c86696bf339baae78b452a9ab14148ce79917d7910c6f4409fb8a8 in / 
# Wed, 01 Nov 2023 00:40:58 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:41:00 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:315f44ac156baefadff78fc8bc8a8a54964367dc79384cc2b2786c602dd062a2`  
		Last Modified: Wed, 01 Nov 2023 00:46:12 GMT  
		Size: 49.6 MB (49612659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983eb873957ff63adeb1906fd4672d8dc3f780ff244183f7cf7e2a2e8607a4a1`  
		Last Modified: Wed, 01 Nov 2023 00:46:21 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; 386

```console
$ docker pull debian@sha256:8ee3628469fa4b2ff564cc1a55a673eb31f871889926020123a94f67973f1dcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 MB (50601063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ca66dbb364fd44c365b4a293f48c49f6102039737bf12da2f46ab1a6b400ab2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:41:51 GMT
ADD file:02448fec868d4ead9c9ba4522890527fae0a8383d230ad96d1332711598c24fd in / 
# Tue, 21 Nov 2023 04:41:52 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:41:55 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:1a62b4e81c4807ef7dce246f03cf8d5229c384cb52b6bdfb7f1df20e7812678a`  
		Last Modified: Tue, 21 Nov 2023 04:48:26 GMT  
		Size: 50.6 MB (50600838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6cd865a296d01caa915fcf79779c4df0c5956e378ca3ffcff89ca1e7818beb`  
		Last Modified: Tue, 21 Nov 2023 04:48:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; mips64le

```console
$ docker pull debian@sha256:b07cd493cde05727e40aae8dcdf2b9afac95cf137b0ff9216bb7f05ccf4feaff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49569426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a98d0c9b4982500fb10abd555efeb9019a3d6bf8bda0672e2adec3fe8cee14a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:13:53 GMT
ADD file:484363709951b76cab1fbf3e7caf4f006bf1917127ca9071365e8ba20c80ac88 in / 
# Tue, 21 Nov 2023 04:13:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:14:08 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:71826ad9cef5309b30c1a728078ce3b7e80a5780a5ccd856baa4c9b62d4dc295`  
		Last Modified: Tue, 21 Nov 2023 04:25:06 GMT  
		Size: 49.6 MB (49569201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ef25057da3fa431d898ed964e4ab60daa84bb674e3b118c298bad4c5726fa6`  
		Last Modified: Tue, 21 Nov 2023 04:25:15 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; ppc64le

```console
$ docker pull debian@sha256:0089455ec515c578003377682d3770c27972f686148f888e23227ecef935b9b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53576088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91050186425ec2441cd5f9db5b9ed0869d6af9c350d41b7527f55b4974d99ce2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 04:25:55 GMT
ADD file:0c91d476365cfc1076554245768ff131f2899b3b3b92d74ab7dcc15a437f21b0 in / 
# Tue, 21 Nov 2023 04:25:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 04:26:02 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:c60bb382b41113221545d52eeea57e75cc0d76f056c6e31a991f40e504b6c040`  
		Last Modified: Tue, 21 Nov 2023 04:31:21 GMT  
		Size: 53.6 MB (53575863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9b3285334dda10b628f8184247c2abf4f5e1e47f3a6ff52ba873f3eadaa06e`  
		Last Modified: Tue, 21 Nov 2023 04:31:30 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:stable-backports` - linux; s390x

```console
$ docker pull debian@sha256:fc3f09a181d64aa037d26c0cd1c5a3f0cdbec35ac47e9b5429beed61d1d8a6fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47943193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a12c985946a3fccb869807b8ea77fb23113b46aceb7bcee136ec02b07a9922c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Nov 2023 05:06:38 GMT
ADD file:2fd0e93b36db470b65ddf3b3154e08fdc83f8c65f16f5dca7aad699d3d818561 in / 
# Tue, 21 Nov 2023 05:06:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:06:54 GMT
RUN echo 'deb http://deb.debian.org/debian stable-backports main' > /etc/apt/sources.list.d/backports.list
```

-	Layers:
	-	`sha256:21aed744c180fed5f9182e7b5c77c7a665599380381860720095e8c30e16661b`  
		Last Modified: Tue, 21 Nov 2023 05:11:41 GMT  
		Size: 47.9 MB (47942970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252b1f491c41ed85897037a5eca99c19d6814f7f48a2da7c1cae7a35b9cd9ef5`  
		Last Modified: Tue, 21 Nov 2023 05:11:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
