## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:04570dc724c369e14d4e3795b2d27224c53d5f15804b642b23ede27d4f45eb4f
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:66181a21c8dd31d4ae5edae847f336f40a424432fd045295ca2e296cd0cc4b7d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.2 MB (68196160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ede5fcc504eb9bd82bb9e34d08759bc407e6b10ebd48bb25994da75baee95f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:20:19 GMT
ADD file:a50affde4f5ccdfd6450a642199121ffc180bb8cace944a55fab7a78ea851199 in / 
# Wed, 13 May 2020 21:20:19 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:27:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:be2ea06d55bb33c31098151d199a24029c4e0dd6bc5b3da9f617bb04e37d79d9`  
		Last Modified: Wed, 13 May 2020 21:26:07 GMT  
		Size: 50.4 MB (50387525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b353a80f0a7f8fad0ab9c83c30a335d821e084c20b62cf5ea881c00f5ee6aff6`  
		Last Modified: Wed, 13 May 2020 22:45:09 GMT  
		Size: 7.8 MB (7812385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f42905b195f8e4cad9788956a131dedb26c1be58f7e369ae2501e029fa863cb`  
		Last Modified: Wed, 13 May 2020 22:45:09 GMT  
		Size: 10.0 MB (9996250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2a8f4c178d1786a30236be21378b212db2163392c20058ef07e1ebf378ebdcec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65151577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f46b0f3d253e83855773668b6c26f61af7ff45b7366405dda1e7f32cf972c0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:49:42 GMT
ADD file:0d750ede80457d700cc7920bf7758097730f05dd745594645d18f752b03ee4ac in / 
# Wed, 13 May 2020 21:49:44 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:31:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:daa20d7c2fc68b19ac519617f67e18594a86dae573165b8260331168fd68440d`  
		Last Modified: Wed, 13 May 2020 21:59:00 GMT  
		Size: 48.1 MB (48105223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1ed27e51f518bb7f9d3d8f217e841fa0e04cec84e4be751525518dcc9a05bf`  
		Last Modified: Wed, 13 May 2020 22:55:11 GMT  
		Size: 7.4 MB (7359297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb6799de4bbd5a170a48ae198dc7bf17edd128910c4afe2e792507f17519938`  
		Last Modified: Wed, 13 May 2020 22:55:12 GMT  
		Size: 9.7 MB (9687057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c54667e7f9980a8f5f48e891481cf6472699191d88aee3cf9f4ef01f9159aec9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62311294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d348616d247718b81cd01981f8b68e45a92cca5bfca9cac22d9c1151982e433`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:13:33 GMT
ADD file:8a00a4e8b308e132c6e665ca4e517d4f8b3ba171a2f539903029bc01271087d7 in / 
# Wed, 13 May 2020 21:13:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:56:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:152c1d0ea8a0c219e7a54e8b39fa0bc45d7a9e072c2388cb928448e26aed5418`  
		Last Modified: Wed, 13 May 2020 21:23:12 GMT  
		Size: 45.9 MB (45871321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bff79e1c1f74ad9a60f91709c157c26840bb33b1c4e92d724bad04374160f1`  
		Last Modified: Thu, 14 May 2020 00:20:12 GMT  
		Size: 7.1 MB (7096779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a316208b08652f2aea0cc849622bf6cb91a53f9b10a9d0892580ae96ebb9e90`  
		Last Modified: Thu, 14 May 2020 00:20:13 GMT  
		Size: 9.3 MB (9343194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fc2c0e145ca90545c87dd989e1af9ff9b9a0a8afbb1d14ea5188d6e11711fcf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66833676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bedb554a4deb0b8bd65adc3d002e1052f1d9964ef022e1feb62d61cf67f20`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:08 GMT
ADD file:685903e2621502d2f743969aaf293a5feab58680a95cd93a5ebf2b07f3b5d358 in / 
# Wed, 13 May 2020 21:43:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:24:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:24:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0be831822ade5f87765ba6ff26243b12a3ecd4c379df96483549a7992c1fd35b`  
		Last Modified: Wed, 13 May 2020 21:52:50 GMT  
		Size: 49.2 MB (49168115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2879905fcfbdfe9945e6eb39396c6b52b929faf145449ab656f7b35bb6387a`  
		Last Modified: Wed, 13 May 2020 22:39:40 GMT  
		Size: 7.7 MB (7681618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2769f7d2af01c05219ba1529b243249dcedccd56fabeee3d41d792b819f494`  
		Last Modified: Wed, 13 May 2020 22:39:39 GMT  
		Size: 10.0 MB (9983943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:018b2a29267735926984613065d599d89af07d6dc017922c80fa19d6d1b299d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69474236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e296eb786d3e99322e031c4bed24a2a49d0302cf033e766fe33efe9ddf9f34b4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:39:08 GMT
ADD file:6aac8e08fe944df3eddb4f6d5754281e407717bf6c2ec1ed9b6ab6af21dd6ee8 in / 
# Wed, 13 May 2020 21:39:09 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:41:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:41:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:adf8f9afd28c61bb1494b99fd6560afa547f46892f87c9847b019ac6d551809e`  
		Last Modified: Wed, 13 May 2020 21:46:14 GMT  
		Size: 51.2 MB (51153891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da0d50611a9ebbc8b9bf756eedd764a8de229bfc658664649463c92bfc78831`  
		Last Modified: Thu, 14 May 2020 00:01:55 GMT  
		Size: 8.0 MB (7981818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32f66937263dbe4d20950081f58d45120003be827ee862cad76fc2f62a25e9e`  
		Last Modified: Thu, 14 May 2020 00:01:56 GMT  
		Size: 10.3 MB (10338527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9fd75869bc6113b4cf40b381210cd498597b80bb62875d5a74d95c8634c9dc0f
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66267365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a6fe919b0a019e958b1c6ae5b668ab5fa0f1cfd65bd6b50666eec56e768da72`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:48:28 GMT
ADD file:97e851af4cc7dad736e0b6bdf3cb1b91e138aa9258cde6c860281333581b653a in / 
# Wed, 13 May 2020 22:48:29 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:57:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:57:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:73ad38a668fc7790605704e34ddd5538366afd1604b76791e166187e503daf85`  
		Last Modified: Wed, 13 May 2020 22:57:04 GMT  
		Size: 49.0 MB (49021790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298d60c32e1de1409e5c95129f71a0e8a0806469bf44e7bd3c1ab4cba940ed67`  
		Last Modified: Thu, 14 May 2020 00:16:02 GMT  
		Size: 7.2 MB (7229789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f486b519d052c2fa785f0c37d788177cec9f73ef162f88cd44e383c2503b553b`  
		Last Modified: Thu, 14 May 2020 00:16:02 GMT  
		Size: 10.0 MB (10015786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e9c85cbadb9dede3ee701f29df342e65c63ee65b0d9e4892bc05c9e16be419ad
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73122901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768a27c5becd22499b08263ef59424cf90dbbac75dbf1d5c35ac5b720856b2bc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:20:32 GMT
ADD file:ed5dc7bd2c0c0dafef9ca4829cd89719c538cd23991fb941589e7fd3bf96b407 in / 
# Wed, 13 May 2020 22:20:38 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:43:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:44:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:19aca0f2a5b89bbc37caa77bbd1612566fadbbce5c3381246fe356d7e5d14774`  
		Last Modified: Wed, 13 May 2020 22:57:18 GMT  
		Size: 54.1 MB (54142914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556cd6fadc0f341d090a18ecfc4b6aedccd3d99f6eb6a336e3bee33f096c095f`  
		Last Modified: Thu, 14 May 2020 00:28:57 GMT  
		Size: 8.3 MB (8252823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633177125031b056c9e79b442829845cc6886ad14d5de3cc2459317eaa054d94`  
		Last Modified: Thu, 14 May 2020 00:28:59 GMT  
		Size: 10.7 MB (10727164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:40212be4a7b3477043f2596938099e931aaa2f474c06bf0ad3a8615e23f06d3c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66229607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:846b5fcfccc4dbb7c149275ff25895bdbe1b6d10e4a69f6fcd0999b161e07184`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:42:20 GMT
ADD file:8f8ce7623c9f93bb85bf3b2bb1f2515de7b053e11c2efc56feb959322aefc0a0 in / 
# Wed, 13 May 2020 21:42:22 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:39:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:39:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6542b1e7bcc740fe79dab47cd5bcdb30fe618acd5d0d0e2583571b2ed256809c`  
		Last Modified: Wed, 13 May 2020 21:46:45 GMT  
		Size: 49.0 MB (48965117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfdd777c0ca04e5c74f52bdae1cc0e2a1ba232e895f109269bf84d8bb598a7a`  
		Last Modified: Wed, 13 May 2020 22:48:24 GMT  
		Size: 7.4 MB (7382349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81be4faee9a8c310dbd16b8d77a0a4eee7f207a8cd04340c0852eb46655b9e7e`  
		Last Modified: Wed, 13 May 2020 22:48:29 GMT  
		Size: 9.9 MB (9882141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
