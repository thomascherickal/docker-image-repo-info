## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:6354f32cf85766e251dad649dd8016bbe296ceecf523482d0c2a8df77bb0ca4d
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:983a53bfb5cec227c03a60190ba42f7ef457c43269aa4bf80c958e907ea9b277
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70401916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2f6454ea25793a0deb0c6dfbc7d16cc92b142239710aecb167c7c2d045c4e4f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:20:54 GMT
ADD file:375c01cd4aba0ddf77202decfeed5df5e3119ce460fcbf1f3b47f540a70b3864 in / 
# Thu, 10 Sep 2020 00:20:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:57:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:57:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:08d7334100fee80149028a0d0df44589b68e0c31592157808d18b68e6a572fd3`  
		Last Modified: Thu, 10 Sep 2020 00:33:04 GMT  
		Size: 51.9 MB (51906528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e2cbaa6fb6571d6e6f88e645061abb7c64ad18e76e900e6cfd8b80c5b36e84`  
		Last Modified: Thu, 10 Sep 2020 01:14:04 GMT  
		Size: 7.9 MB (7866624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f330112cba767d415d7e4179b0dd52578b7685d2984ac61d9c3ba0884843a`  
		Last Modified: Thu, 10 Sep 2020 01:14:05 GMT  
		Size: 10.6 MB (10628764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ed9ccbfff779a62f91961710d791145443df6e6bc429bca5f8b6de0469d8c041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67627368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa37aa1a3ad9ba7e9cb6257ca2d7a6092ae95d9903941402c40fd0039154c4d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:26 GMT
ADD file:f71e0d87d6d096130aa8dce14ce4db75b3a50725e9ba2aaab46f722a444291c9 in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:27:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:23e3aed2d466532e16ed7a54a2dc8d1ab497d8cd849573a7aa149e39f499eb77`  
		Last Modified: Thu, 10 Sep 2020 00:01:42 GMT  
		Size: 49.9 MB (49868299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57296d1a05acc9b2b6a146828bc5cd73f18a33087981038e29d2911236360b77`  
		Last Modified: Thu, 10 Sep 2020 00:51:46 GMT  
		Size: 7.4 MB (7444028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf329ff0c0ac4aa69298e3dae2a5539c0c7f11957ec83f3ae34b781fe1af258`  
		Last Modified: Thu, 10 Sep 2020 00:51:47 GMT  
		Size: 10.3 MB (10315041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0a907fb47131937e9dfd3693343bed868ae85ebcfba365df3f397e4455fe4b40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64730062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85a0034c1b8bce09a56db1727fdb1d02615f462bbb5f0c988f284028f972accb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:55:34 GMT
ADD file:8d817c9168a8bfbddda5007f76443d27203cb5bf02ec609cd277ddc327736b10 in / 
# Tue, 04 Aug 2020 04:55:36 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:45:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:45:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:984ab044320fbabd5c060737e15adfea7aa109893b7f68f41abc04f445d3440f`  
		Last Modified: Tue, 04 Aug 2020 05:04:18 GMT  
		Size: 47.6 MB (47570419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93473ce552fd633dff0ed8a7eba4610e368b271c6582de1c474472a31cc7340c`  
		Last Modified: Tue, 04 Aug 2020 08:24:12 GMT  
		Size: 7.2 MB (7243678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9559bb2ff9f55098d0aae9e6210eb73fdb47f91e0b6fff535ae21fcbbfa54dea`  
		Last Modified: Tue, 04 Aug 2020 08:24:13 GMT  
		Size: 9.9 MB (9915965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:35a5885329a6dbbb07c536a70010845ea21cc1b981b64dcfb67adcbc8623afe9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69204517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:987a312453e6e6a41af020dae3c276409466979d39b116d218e63e5704a0980d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:49:11 GMT
ADD file:82c33a26fb9be3ddaf17956539af2b205bdb6e28fe5ff1c7304ae8f294fe9581 in / 
# Wed, 09 Sep 2020 23:49:14 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:5a65667356fa05b061c6733c879afab36ec44c6877341c2527e321b7206a26b2`  
		Last Modified: Wed, 09 Sep 2020 23:58:05 GMT  
		Size: 50.8 MB (50825395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730279b4ebb859065c90bbf90b3ac77059bd7d1e6cdc143106e0994dca9f4c59`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 7.7 MB (7743447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2c8b657c8d1b22dc8f6d15821f7035a315a0900f84b26ef36c86803feb02c`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 10.6 MB (10635675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:7d9dbfdffda026db4f4bc6992a7f5ba0a9736a3b91e67d06a5db3d75b468022a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71969620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5450c90d662e44d72885e2bfb547b02d950e88634d8c1961584aa9e3dfdff24a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:36:50 GMT
ADD file:e3f476fccb15ccc08c3c8c26ac23f1909e7c0f79bc060289f35fc37bb4483f80 in / 
# Tue, 04 Aug 2020 03:36:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:04:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:04:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:308ce7c38ffec8ca43e219653810c298ee87abfaaa068ff112f1e8003b108546`  
		Last Modified: Tue, 04 Aug 2020 03:41:50 GMT  
		Size: 52.9 MB (52909727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429c636a1f75410c98b200faef3ff9f568a242579e0d885a7b7c70d771f96e9a`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 8.1 MB (8099324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e845809b7e141a8bd0e85748582037ea1e08bcb9ca449097624dfc315d876d2e`  
		Last Modified: Tue, 04 Aug 2020 08:24:23 GMT  
		Size: 11.0 MB (10960569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7f7605f9ca2196625517871a1ba2d0dc6f3731a0512c3a3c5d88caa761828051
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68600344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7792a320a2fc82afeca15f8d402bf74a3d0798c1e1dacc45d652f72015973dfd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:41:13 GMT
ADD file:9e3d31545fae8b44e8aa3ad24629d2336276c01e23dfbdde9885d01e61a54298 in / 
# Tue, 04 Aug 2020 06:41:14 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:33:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:34:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:249c58d6beef4ec2d380f0e2adf7ea99a80c295cddcf6f6bc3d6b463dfe44a05`  
		Last Modified: Tue, 04 Aug 2020 06:46:35 GMT  
		Size: 50.6 MB (50550783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049f809de28cc8d8e169ab9ee5721613f58fafdc670bbe6d66a1058fe998ee06`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 7.5 MB (7450522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557e2093dc94091a8f931745b728c83f35ad977f14de65f1ec5db00bedf8580`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 10.6 MB (10599039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:67ad1dced6dc489dd9af29c4fc5e5c94d219703bd8cd2f641fbfd2acdde2cceb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75330755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19f2a92fff074c72572dfb53df34eafb1c31dbfb6d766ce865358c6e740d8163`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:43:52 GMT
ADD file:a1065b5d1a75daf3153a753a23c630c5a77451644b83418dd23b2c1d046c970d in / 
# Tue, 04 Aug 2020 04:44:00 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:01:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:02:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:26d0cc426ef5200b8e12941b37f3b65f8de8a01be463ecfef94be00ae56f5596`  
		Last Modified: Tue, 04 Aug 2020 04:50:57 GMT  
		Size: 55.7 MB (55655910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aadce00449a8701783ecb72b8dce872a06609d7a90a69b4dfa29a8727a1bc3`  
		Last Modified: Tue, 04 Aug 2020 07:42:12 GMT  
		Size: 8.3 MB (8347825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f8213614f8c61ad803c5be08bb2ca48b08b0b8111551a50801c69e31afcf4b`  
		Last Modified: Tue, 04 Aug 2020 07:42:13 GMT  
		Size: 11.3 MB (11327020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ee809f5a4ba794419fb939755e2dfb26f2ce6c345fde3cab40cad69f4f2f0e26
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68511194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8de6252a44f4d8218e1512a21cfb7b7a6fc7c263a743bb9c1e071dfdd1de03`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:41:38 GMT
ADD file:d30705fcc57734260b517d32c4d610f1fe18e7d5faa78a22754774f5bf15eb9a in / 
# Wed, 09 Sep 2020 23:41:41 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:04:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b7fac0c9089d6ff39f6a7de3af657a8d580a7b074b45118b115539fd90213654`  
		Last Modified: Wed, 09 Sep 2020 23:45:45 GMT  
		Size: 50.5 MB (50468550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e4abf36c400373c14e1dc03dc7d41c9bb01249ef118a39b67294471b0cea9d`  
		Last Modified: Thu, 10 Sep 2020 00:11:24 GMT  
		Size: 7.5 MB (7537717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c291ff634945f7dc165f540d95c5d3958483aba31d45fbae0ee30d37ef13ca7`  
		Last Modified: Thu, 10 Sep 2020 00:11:25 GMT  
		Size: 10.5 MB (10504927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
