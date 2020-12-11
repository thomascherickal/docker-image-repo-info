## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:8303d955ebf47b6e8163efb331b58ba4338e09616ac904688fc69d60eea5303a
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2ec8a6bd2a2877a009a9e59778bc626f974ef251fd5a3167b8332f6da0eeb824
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71688175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e015d485fa0e676e79f1a5c345e35f6b1016d25dde9caf17af492152184a918`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:09 GMT
ADD file:e5210ca55e6714aec9564543eeb4b4a748c57e62c0ae0c741dd0f3eb75ab72de in / 
# Tue, 17 Nov 2020 20:23:09 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:39:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:40:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:648de6ce4c8700aa65bb00de61082bc80448ba5410d2558ccd0f8c5e5616dbdf`  
		Last Modified: Tue, 17 Nov 2020 20:29:13 GMT  
		Size: 56.0 MB (55978493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330a58a1358b2808071560abfa71693ca944d1732a1543c107859d521b29bd65`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 5.1 MB (5063542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3e6e253f47148f777fe41db1237b0eba7f14df71ec26f973f35c05182b4173`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 10.6 MB (10646140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:106550b1b20cc4e0110a1b1c80799046c4ca426001b123e5c49fd15e8b190e5f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69087855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d19cf9f06699812ebfb364662009b82d8d88649326436d41d70425f2b5111097`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:43 GMT
ADD file:a57353f597051225232a9e7abed847b86e4c6dddd2072732b4625acbac7128fd in / 
# Fri, 11 Dec 2020 02:07:47 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:50:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:af6b8b544b162386c7b3c6d5c131158e341ff3b454198faf077cc6c1427321df`  
		Last Modified: Fri, 11 Dec 2020 02:17:13 GMT  
		Size: 51.3 MB (51288429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e601c83f1a1756a052d156762b6629539a7e67063cb8852d73fb18958f7726`  
		Last Modified: Fri, 11 Dec 2020 03:08:38 GMT  
		Size: 7.5 MB (7464314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6a25346e41f4aa7fbe4f2fbf817bc776305935298bbe8403d2b5fd5ebec3a8`  
		Last Modified: Fri, 11 Dec 2020 03:08:38 GMT  
		Size: 10.3 MB (10335112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3f5b438dfde3a30914017aab51d2a25a616875279268c6a6db5a27f18b251eb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65936251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe40ce14727139636269cc766467a2835193b5cf7afc28ed7d1c84b0860315e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:06 GMT
ADD file:7bc088cc808b76314a338212bb2b1cfa40e3747a587709f883b0b3d24272ed5d in / 
# Tue, 17 Nov 2020 20:24:08 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:52:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6540e01ce43e9b114890e344f5358356defa70d487f91c1a002e0a64db73d60d`  
		Last Modified: Tue, 17 Nov 2020 20:34:10 GMT  
		Size: 51.1 MB (51125953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba56633e4f20c85ff3a7a96ebf325e3b8eb38ce01b4a19d147fba95c41307d6`  
		Last Modified: Tue, 17 Nov 2020 22:10:06 GMT  
		Size: 4.8 MB (4838976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f95259ef99cc96a3d8352c48117cd75a72bbd30aa5c3198adc601ee244ce8`  
		Last Modified: Tue, 17 Nov 2020 22:10:07 GMT  
		Size: 10.0 MB (9971322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:653649165e85305ba91ed15c627e09c9a931aa9ce739ed336f71c10063ff6b07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70424241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5161dc23b84d6c5756111f2477170e7920d5e43c54dc93115ed3855ff3455d7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:57 GMT
ADD file:dd38237d30f418925f9d05a463817130964bc613d39a38eeea7b87b9b5d62608 in / 
# Tue, 17 Nov 2020 20:25:15 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:24:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:24:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:28adf41b7f9d0f64232c0970a16416d0ef2eaa00df57f3caf5d257ccbd3b206c`  
		Last Modified: Tue, 17 Nov 2020 20:33:04 GMT  
		Size: 54.7 MB (54719929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516539a7ff1b41bcd60f56a25019366722df8db637f7a409ba85ab9918633b31`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 5.1 MB (5055909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58beb0eca7357870a7d9572e6897310b7dbb65ea59a9f76afc5b75a63c11820`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 10.6 MB (10648403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8c9f792df88c924d883281936dd7ae7e4a3b7328537eca3b8080bc4d044f1fd6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73308219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88329186fa891b9f9fa60ba923532e1c54ad8595d6bbf2a6986435c553ed2f82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:59 GMT
ADD file:6d6afa8490ae5ac639c8369b0f5d9f8e49c675672ebd5348a955a3c9656453f5 in / 
# Tue, 17 Nov 2020 20:22:00 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:17:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be81561500ea27b67d364b1567d73e6fbfac19e1739e5b1e5674dbea758abedd`  
		Last Modified: Tue, 17 Nov 2020 20:28:52 GMT  
		Size: 57.1 MB (57102236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc436cb880e1d23236f4f748fe380b16b0e16955049a2c0c1ab65456f67c2a49`  
		Last Modified: Tue, 17 Nov 2020 21:26:18 GMT  
		Size: 5.2 MB (5183137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca3e53afca84ddbe3333e0b6c779a68bb454199b167cfb74eda23f74fbea675`  
		Last Modified: Tue, 17 Nov 2020 21:26:19 GMT  
		Size: 11.0 MB (11022846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b20c27c4b5d424f699dafdb40897c11674231c2f4c406ef97135b52e30ae4514
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70157304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:736fd42e2728894d1a8f81e87838dddf049f5998fb4060065c628322bd8e256c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:55 GMT
ADD file:144f263fbf8197586830814ff675d3c7d3ac8e3df7debe6633a1e91f84ff845b in / 
# Fri, 11 Dec 2020 02:03:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:55:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:9b60fb1f705939e8d3e124cd99cb825ac48613619a7a75de5656f0bde8bb1f05`  
		Last Modified: Fri, 11 Dec 2020 02:11:04 GMT  
		Size: 52.1 MB (52069726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc2b81267c2dccbb94aa4a39fbd561e967b04505581d2d37c94c116454be253`  
		Last Modified: Fri, 11 Dec 2020 03:05:44 GMT  
		Size: 7.4 MB (7430898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d8b7d4e3509bc9ab5283dda924581973c2fe390d34bf794abb077b094d9c66`  
		Last Modified: Fri, 11 Dec 2020 03:05:44 GMT  
		Size: 10.7 MB (10656680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e24af2899ebd7d1a555cb3049f3d97bb30a5ce2905dd761ca53bb517f7a992c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76900342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29e0eddd5ae5857fa2e8800306cc175ab37a0ecd4617edef6b92b52eec3b99b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:29 GMT
ADD file:d9f4936d2b1902ef4008c438adfc5b11813d611494bbe59a59f77de4d57c5c8a in / 
# Tue, 17 Nov 2020 23:23:40 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:24:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e7c5331f40f844384a2b7c7835ce9547f6d5cb22a3b99e72b08ef585bea2c3bb`  
		Last Modified: Tue, 17 Nov 2020 23:34:29 GMT  
		Size: 60.2 MB (60189345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c542ef20d7487b58e220d23902720f3093c22a2ac72bde481e08d93fac8c924`  
		Last Modified: Wed, 18 Nov 2020 01:58:07 GMT  
		Size: 5.3 MB (5302640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93377737fbee467c96f243247282c2535ef88e661736d10f42cdc6bc9e340f5`  
		Last Modified: Wed, 18 Nov 2020 01:58:04 GMT  
		Size: 11.4 MB (11408357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:12dd0226821fe2a3ff63116dd0a60c01d12b9bc10d70736470f6a39e2f1dbf3e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69777453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf07845427e81d6f0b253cbcf5514ca8551367e7412e5747a21cba8304efd257`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:51 GMT
ADD file:8962f20bb4a72e135379229e0846f699624835b74ec331608abaaebb561f33eb in / 
# Tue, 17 Nov 2020 20:19:00 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:36:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:36:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ea0b76bf69e10e271efafd881a3e6209b856a27b396fee1fe5c96626da5668da`  
		Last Modified: Tue, 17 Nov 2020 20:24:00 GMT  
		Size: 54.2 MB (54214424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d6fd966df630924882593f8be50b60b4dd8cbe08956bf3a1a09ab0c62129fa`  
		Last Modified: Tue, 17 Nov 2020 21:54:49 GMT  
		Size: 5.0 MB (5048615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5387e7afec1cae76ed6c62c9f9b187efd32793da95a21fba4cd0099aa37002c`  
		Last Modified: Tue, 17 Nov 2020 21:54:49 GMT  
		Size: 10.5 MB (10514414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
