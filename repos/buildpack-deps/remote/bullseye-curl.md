## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:832525da4e87a3e7bb040b1e294d55284cac0976a819a0d350e713158d05b4a8
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:05cbc03021958d3c23ea2038ba6d328b313278bb117dbf350efea861f0d70635
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.9 MB (70920531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6706d8c66a77dcc1e4d32d09391eb16841422137070394c2286115b9bb63e681`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:19:59 GMT
ADD file:eebf6f761892ad2407885aa93a2abf7647cf0367e3590f3cc7971594ff47193c in / 
# Wed, 23 Jun 2021 00:19:59 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:51:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:51:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d28ba3bddf26336a2dff9ce3319ecd166971168469860f171fa659f62cb3ff6d`  
		Last Modified: Wed, 23 Jun 2021 00:24:24 GMT  
		Size: 54.9 MB (54898218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf411e1e4e47abd58ba697cdc3f8f769d452520d81804d6260ac2edb014fd41d`  
		Last Modified: Wed, 23 Jun 2021 01:00:26 GMT  
		Size: 5.2 MB (5151216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab85705b51fb188c0567dca75cc18291fe81258917cbae6ed4d271ae1e1e1d`  
		Last Modified: Wed, 23 Jun 2021 01:00:26 GMT  
		Size: 10.9 MB (10871097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3510d5d4ecd1a999a1da718f4b74c22d724fed84f0843c3150ec55696b4b430b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68071400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c687aeff2c42ea5a53f3eef65a0931800d58173594580dd50abb6f25f60e29a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:53:46 GMT
ADD file:776704b0dea7e9c9856d53c5db99eb2cac12414a59e66258c549cd32602f5f15 in / 
# Wed, 12 May 2021 00:53:53 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:49:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:49:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4470c8b9361b9718aac07fcf9a711d40000613ef3e0f694e3da9f5ae091dd9ff`  
		Last Modified: Wed, 12 May 2021 01:08:50 GMT  
		Size: 52.4 MB (52439186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763873e8e180836bcde25dbc607672fb53b7253594d501513fb643acf8f441a6`  
		Last Modified: Thu, 27 May 2021 20:03:02 GMT  
		Size: 5.1 MB (5061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013a6f9785a03eed88540490a717438ff240f3a58e51af2ded1a200398a169ca`  
		Last Modified: Thu, 27 May 2021 20:03:03 GMT  
		Size: 10.6 MB (10570295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:36f18344d3d57317e3a8df5cfb4a8c57f99cf79c0343522f0db2c4304d4380c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65239118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:159df870f757b20dad2b20bdfb094c8f9e0ef0d85dcad1489b99dba735d32900`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:00:23 GMT
ADD file:8ed6f13e7955c981e57f2e063b7bfca16927ded9fed3cbd231923f2fc092555d in / 
# Wed, 12 May 2021 01:00:25 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:37:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:50de689ded7920797496a1e9f831f07c907224f7c629bb02a03a96ae30d367de`  
		Last Modified: Wed, 12 May 2021 01:18:10 GMT  
		Size: 50.1 MB (50101718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eadd03179b184db82df36753465390a99da5b2ae95dc934fcd05fb8fd8a676b`  
		Last Modified: Thu, 27 May 2021 01:01:22 GMT  
		Size: 4.9 MB (4921246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10155d4071aabcf375a96f3b69b17f5e9cb5e2f69cc8fea2cb2d87c0db3fa24b`  
		Last Modified: Thu, 27 May 2021 01:01:23 GMT  
		Size: 10.2 MB (10216154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37e46c9829bdf4c17069cd428c7d7d7363c232777fcab08907047ce2cb5e8ff9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69594985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7527d1485195c29432b613858f0575047c5a9595efccec47623de4146cf9cc9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:00 GMT
ADD file:4a6460733f3542d1957e24a1b1640ad7a76b0e4d8aee727e7d2ad9ecb8baa5be in / 
# Tue, 22 Jun 2021 23:49:01 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:23:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:764e5bfd58ff2b8baf2ec95af0b179082665955a271e28d9b50d4ff1917c2c0b`  
		Last Modified: Tue, 22 Jun 2021 23:54:07 GMT  
		Size: 53.6 MB (53582009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61ea5376efdee8b03645276110ca156d0bbdd3889e467593830f7e683fedabe`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 5.1 MB (5140889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba64b692b9483da8feea34bf3f3f5f6650d0883ba74afc0083588f0a5e6219a7`  
		Last Modified: Wed, 23 Jun 2021 00:32:01 GMT  
		Size: 10.9 MB (10872087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c7a97fded446d24fc59e9536a2b9bcc14bc4e2139f46b9c2372e1688eb00d142
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.4 MB (72445219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:342414710e97cb031e162031760056bee61ee5db1f5dcdd1b42bbef91f0d860a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:38:49 GMT
ADD file:ed43ceae72cd0b1a1ee0ecf4319bf0a9ff0d8cc4542a983609d4df18ccb3133e in / 
# Tue, 22 Jun 2021 23:38:50 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1a1a10c368f246da8fdeabb7eecba4e66e58cdc28feb3b3f7714896e4f52dd56`  
		Last Modified: Tue, 22 Jun 2021 23:44:57 GMT  
		Size: 55.9 MB (55914378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8155b7693984d8cf280e3297045a2d6e4381a5942504ce0cd264fc90f9d3adb`  
		Last Modified: Wed, 23 Jun 2021 00:16:25 GMT  
		Size: 5.3 MB (5280678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8daea17889b2d1f7c6b1d266c5f433c93d238bf490f3cf4f26ffccc30ee4600`  
		Last Modified: Wed, 23 Jun 2021 00:16:25 GMT  
		Size: 11.3 MB (11250163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:df3711adc2b456f283e7e49f67fad0503b5950440c802b2f56a765d1a6beb041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69139425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6d817517c52679f0b27911f64fb7966114ad8f3d54e6c9080eb65223f8d860`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:08:19 GMT
ADD file:c35f12783d634fefd92f2d45605502f97a497b66a15f60dfccb4b2a2d4a293cd in / 
# Wed, 23 Jun 2021 00:08:20 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:37:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:37:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:3ebc6252e914164fc2a31f5418122631ab0e70c83ecb8f8b24f7e1ca5f4f2fa1`  
		Last Modified: Wed, 23 Jun 2021 00:13:48 GMT  
		Size: 53.2 MB (53152965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fcef1ce2b6c14e25f573bcaef690fda6b4e405c35a7b1b8952b7b62c3c8024`  
		Last Modified: Wed, 23 Jun 2021 00:50:30 GMT  
		Size: 5.1 MB (5113563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec06bd468c211fbc95164b859ed15795c4a88ea59bad6a4f3e2ea99c8f83804`  
		Last Modified: Wed, 23 Jun 2021 00:50:32 GMT  
		Size: 10.9 MB (10872897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f1fe65a606cece8be98abf4ea7a9f59a2bc7ea35d949bbc8557962ef79d0df8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75819911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a90dda2255705b740fc852e13f15c1671d0727243a19cfbb5d05b6ad515cd0c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:32:59 GMT
ADD file:dd3e802ee39ef6460fa54303399ebc1f08919c4011f872a9ea00cdee78e2e6eb in / 
# Wed, 12 May 2021 01:33:04 GMT
CMD ["bash"]
# Wed, 12 May 2021 03:14:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 03:15:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:79c001f710a199bddecf6231e4c1152e873413174cb20e083729089e3d15e400`  
		Last Modified: Wed, 12 May 2021 01:41:18 GMT  
		Size: 58.8 MB (58795251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c772a696fa0c3a04186486f51e28b635be426e19d28f70066ae4451f4cdffb8e`  
		Last Modified: Wed, 12 May 2021 04:15:48 GMT  
		Size: 5.4 MB (5399466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b13560e5ca42c500abdc25b1eaba62e4eecf6c07847e8a5ada379658a0a0b10`  
		Last Modified: Wed, 12 May 2021 04:15:51 GMT  
		Size: 11.6 MB (11625194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f63332860401817090aa7507dc276c428ea26eb1119545efe3b37ad6deb661d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69077869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da1df1f22c5e3c40e0c93adfd8e05d0afdcc8e49f88b2f7898477c0f210fa11`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:45 GMT
ADD file:c4e658e7b0a2f1bcd1adbc3f8d4b90c39d22edd3817e41078cce53daa39778f0 in / 
# Tue, 22 Jun 2021 23:41:48 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:03:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:03:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:616c5ebef764d038df48c869a270b4c696a19212343d41c89f2f771e65bc2219`  
		Last Modified: Tue, 22 Jun 2021 23:45:00 GMT  
		Size: 53.2 MB (53183223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ba372b2a518f01bf5ef5547922449c0f61a5b6b5ce8af4f7f223a0acd13e3f`  
		Last Modified: Wed, 23 Jun 2021 00:11:16 GMT  
		Size: 5.1 MB (5134548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2b0dcb7538f1dea99896f8ad049a4690dc6d85a83e22119c18db98c8ec6b78`  
		Last Modified: Wed, 23 Jun 2021 00:11:17 GMT  
		Size: 10.8 MB (10760098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
