## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:55e8b08399933366af5bf7339d286a42b69484a144be7a9505b9652bb3abc9d4
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

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0edf02c125a1738634b314fe74509188fe8ec80d4fe0e5dcb6a8e2c69b752eda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.0 MB (70957967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4210c06ad2290080f1e15b81fcab4884d6d092607663ed35830d2cb7f05d88df`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:30 GMT
ADD file:5259fc086e8295ddbf02e48abef38e9bf93a183079d3631aa7a59306b7f2f9df in / 
# Wed, 17 Nov 2021 02:20:31 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:647acf3d48c2780e00cd27bb0984367415f270d78477ef9d5b238e6ebd5290da`  
		Last Modified: Wed, 17 Nov 2021 02:25:17 GMT  
		Size: 54.9 MB (54932774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02967ef003473d9adc6e20868d9d66af85b0871919bcec92419f65c974aa8ce`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 5.2 MB (5153337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ad2231829e42e6f095971b5d2dc143d97db2d0870571ba4d29ecd599db62cb`  
		Last Modified: Wed, 17 Nov 2021 03:23:07 GMT  
		Size: 10.9 MB (10871856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8f64ae6a92bbcdf3bd87aa336ab8cfbe025c94f2871fb30c7c869ddf5b398637
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68087009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c0670207bd3308452b37f769e1991141d3955fb9c449d6651538516664d78`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:49:54 GMT
ADD file:b9969604315238de271e1769a4b8dd85cdf0d33f9fac387e940d5195ac3030a1 in / 
# Tue, 12 Oct 2021 00:49:55 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:40:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:41:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a97c782f2538791984ce12c859cada96e395e3950d4cb7d1238e08acd2eb74ec`  
		Last Modified: Tue, 12 Oct 2021 01:05:12 GMT  
		Size: 52.5 MB (52452198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34dc529b005dbeff70906cd4baf2310c918ae6379fdf53ef632c3cd1203aa38`  
		Last Modified: Tue, 12 Oct 2021 06:01:18 GMT  
		Size: 5.1 MB (5063794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2876b7f933f68a5b4f35f854cc8c651bf3d21476fe2bb0a786e6376f389b44b`  
		Last Modified: Tue, 12 Oct 2021 06:01:20 GMT  
		Size: 10.6 MB (10571017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e0db5a4c0ddaf3021a476cd83cb48a47baae27cafc02c61fd6151c2b113034fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.3 MB (65273899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a096ebca0a1dcf6c812935690d2f1ceba23cdc7565b5dedf1b01adb266c3296a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:07 GMT
ADD file:43b45f65ff4ba720f6f9a107b5f80818d5ea6ebc4835840b11e9a506351da32f in / 
# Wed, 17 Nov 2021 01:59:08 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:41:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:42:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:dbbf55137aab3c7acd1e012a70f1ea1adeaef8d39b474829965d3480a02bf572`  
		Last Modified: Wed, 17 Nov 2021 02:14:27 GMT  
		Size: 50.1 MB (50134152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1ae7a04cee77523f9e09a62b28632c56a700d0c481be7cddc566c835e7a71d`  
		Last Modified: Wed, 17 Nov 2021 03:04:13 GMT  
		Size: 4.9 MB (4922782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66894dfea839186e94448f6c25a37c6b3b1b42cece6332cc9d36336917e18a4`  
		Last Modified: Wed, 17 Nov 2021 03:04:14 GMT  
		Size: 10.2 MB (10216965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c52337b05fa1f275820e562dc39597db3ec027dbc6930cd6c1424233776c385c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69212541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638dd156261f84c328de4551fcff54679fa0628f7b63b62344e169cb0cfdf82c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:59 GMT
ADD file:eb667e18226da8a1ca5a41beacddc65cd1efec01c3d01e50845c5e89e91ea17c in / 
# Wed, 17 Nov 2021 02:40:00 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:26:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:26:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce18cd0ba11c2dfa8c1a2d2b325e1e019b14d4ae25ffdeffb0f9686c5496bf5c`  
		Last Modified: Wed, 17 Nov 2021 02:46:45 GMT  
		Size: 53.6 MB (53619024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f138a340a2373acc72dcc4ea9ef08bdf5648aabc5fe08f7e8d25222ca63b7ee`  
		Last Modified: Wed, 17 Nov 2021 13:36:26 GMT  
		Size: 4.9 MB (4937639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34c030205ccb8656e30a58f96bb1edbe7c59bf17f3329ae3c442ec897f2b270`  
		Last Modified: Wed, 17 Nov 2021 13:36:27 GMT  
		Size: 10.7 MB (10655878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:307bd4c6b80d221cc5ffaa51a6561a19f142cbe2349df40cd823c45df8a66d0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72457220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1fe930770d8d6583e5406717d0128e6efa4aa9438733ab028c7df182c036184`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:30 GMT
ADD file:e007d6eff02dbc696e1166db315b97a77ae8aa65f2e66ca8074765dde9c70a59 in / 
# Tue, 12 Oct 2021 01:39:31 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:36:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6911c8f66691266d86e2cafa67ca005d919f357436fac971c694d37625b5ba90`  
		Last Modified: Tue, 12 Oct 2021 01:47:06 GMT  
		Size: 55.9 MB (55923419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a0f31369a20c178b1d5c84f192412ed962068e8932d5821eefb00bc7d1cbc1a`  
		Last Modified: Tue, 12 Oct 2021 04:47:26 GMT  
		Size: 5.3 MB (5283102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97aa3d222d7e8d6e0b06e57e5bd03168c422475942f92d09a487bd98d09bb742`  
		Last Modified: Tue, 12 Oct 2021 04:47:27 GMT  
		Size: 11.3 MB (11250699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c8e1c20d487b63fa0111dd8c6dbb3e8cad660d4ad92dfedcc288dbcf88b52ae1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.2 MB (69172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01b4e0250266355d14651090fbb68f4b5950f1e1e3e93ad45e1d024d3e8db78`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:09:46 GMT
ADD file:2971df49f24648b8d5166d87e392e2547d5b03469356f20d112ce6feb3c329fc in / 
# Wed, 17 Nov 2021 02:09:47 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 08:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 08:30:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b095a0b63d99a4c4cd9c1c353f381a69ef041e6f80798d807ae51a34b04920a0`  
		Last Modified: Wed, 17 Nov 2021 02:18:22 GMT  
		Size: 53.2 MB (53183806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2e37aff1692726b1ea3dd0b4eeb684072527295f8e981d3c45825327daea19`  
		Last Modified: Wed, 17 Nov 2021 08:45:38 GMT  
		Size: 5.1 MB (5114925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d4c0302ddd7a6cb573a156076dba9c593e09a0c321b32ae0f1da2bd36bc754`  
		Last Modified: Wed, 17 Nov 2021 08:45:41 GMT  
		Size: 10.9 MB (10873360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ffc112a46cd4cb66176c5d7b815903b1652b33a26fb9f38d3233e1892293d496
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75847521 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cfe935fd31679e71de8a6756361a413d64351be692488a2fd6c0de16648ada`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 03:27:04 GMT
ADD file:85375acb19da58f9eabaa67f8cb425cd1ff2dadb2888bbd9dbfa6223d16fef23 in / 
# Wed, 17 Nov 2021 03:27:20 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:40:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ede9cd7c8f1d380c971a130fb3d8a3914bf3a9106702164c23b2cce536fa618c`  
		Last Modified: Wed, 17 Nov 2021 03:52:39 GMT  
		Size: 58.8 MB (58819505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743814bfd79326104da0238d8edced6b14f63b95734b6dc0e2b7a9d83356b0cb`  
		Last Modified: Wed, 17 Nov 2021 08:25:58 GMT  
		Size: 5.4 MB (5402000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca978d94a6543bbd1c60026602b64e810b4bf65e052dcf19adf2b4d6b518bf8`  
		Last Modified: Wed, 17 Nov 2021 08:25:59 GMT  
		Size: 11.6 MB (11626016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:864eebbaafc1154c0017d16100182a15ea13c7dd81a1e2474b581c03a8e4d27c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d1c13a820b2c0e693a7fcd87c7888df8a0f95367ff8e2381ec07faf8e711307`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:07 GMT
ADD file:b7524e775a2033d246d1096765a0eb6eaa5ba6ed6c8b395522579d2c4e7a2e38 in / 
# Wed, 17 Nov 2021 02:42:09 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:07:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:07:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ffa47acd07831fbc96680a705da20704bac0016c20dc3c454ecd45cda44b368d`  
		Last Modified: Wed, 17 Nov 2021 02:48:05 GMT  
		Size: 53.2 MB (53207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c950336719691da019c99e4ff78fe559ab0308ea145757994bdb7be34c6d224`  
		Last Modified: Wed, 17 Nov 2021 03:17:18 GMT  
		Size: 5.1 MB (5137199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d769af2ca44d1c7c206e7190cd71df7cb5ff3df2dd45e1dd52ea447ffb547b1a`  
		Last Modified: Wed, 17 Nov 2021 03:17:19 GMT  
		Size: 10.8 MB (10761499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
