## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:bfa9453529c1311886e6e4f42f732c1fbd55a1a800c3ebd317afd18ac7dc7b92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:38ab4de91420b9d4b14d2da812ed8dfc7cfcc19c7758aff37546fefcc9317fbd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69663636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:772b2b910eefd485a65f9db178d23dc13df4db9cbd52b50caad1849a411d0677`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:06 GMT
ADD file:fd0aa728e8273d308f539e701d2dc6e8058f6e92ecb059335ffe63875d85ce41 in / 
# Sat, 01 Feb 2020 17:20:06 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:16:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:16:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:97a0a01813cb1683b6e005ed8f5c8b75a75a9664de6813860fd76e3186dc8276`  
		Last Modified: Sat, 01 Feb 2020 17:25:37 GMT  
		Size: 51.5 MB (51490749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a12c6dc4c9c9d70ac367f70168220be374ebe17c12337eafde440f00bda1d36`  
		Last Modified: Sun, 02 Feb 2020 00:36:43 GMT  
		Size: 7.9 MB (7919836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a8dbcecacf90650f05d148dcb2f5a0137f3bfd822153d768b6927ec64933f9`  
		Last Modified: Sun, 02 Feb 2020 00:36:43 GMT  
		Size: 10.3 MB (10253051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b95b2cd5f420bc803457d6698f352036958f4fb15435d702d08eedb99d5df6dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66948126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d173f8a43906b5f2335286e6f97167763a7807dcb822aaf24914bbfc4b16e2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:49:39 GMT
ADD file:b4c3e18bbf2b51c4f777d44bb8ef76a6fd78e8e9e057ffeb792fa8e041d3b40d in / 
# Sat, 01 Feb 2020 16:49:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:1758f12059aa2a6d57dcc649233827a3b49cc528e7868081891f2a12944a479b`  
		Last Modified: Sat, 01 Feb 2020 16:56:07 GMT  
		Size: 49.5 MB (49485065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449c159b35252b02eefe1b4989bc90d10d35fd6d17600ae5d662ba279c259ad`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 7.5 MB (7494059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a6070fc56cb0dfa20ffac6472ce9dc9a8aead19638f495a62bff5206bf6ec7`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 10.0 MB (9969002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cb689033d355e9ce2e6943e9bcdf1c333dc1d7b03c7c8a13f5e8e826c6eac863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64097968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997ab0a95f9abaf0e52cdde20965952ba2e5793ff3a8ccd0ff601c4336142120`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:59:25 GMT
ADD file:202d96a6d5151b70202bd50e4082c0330e7568bfc44df705d81cfbe26c89ced3 in / 
# Sat, 01 Feb 2020 16:59:27 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:56:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:39368978c6fdc2e48756694e0bc73ec7a7db16e571f02e42ebde72a690544bc6`  
		Last Modified: Sat, 01 Feb 2020 17:06:52 GMT  
		Size: 47.2 MB (47233777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0657bdf1da7571cddc6b267a05d66156f8304de06b121de57f07153149a8ea1`  
		Last Modified: Sat, 01 Feb 2020 18:24:28 GMT  
		Size: 7.2 MB (7233949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4016dec180e52c4d1cb0efc60d7bce60531a204bae8eb6ff5259e9125ddc577d`  
		Last Modified: Sat, 01 Feb 2020 18:24:29 GMT  
		Size: 9.6 MB (9630242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5c7925481be4184e4fe86c51e55d55e3877fdd41b7332296a35b44162de8776d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68491816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9cf4b0a210d658f05f239ed78a872468f789c3926d0089c0584631f755077d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:13 GMT
ADD file:485f0f88566199683d3683f547dbd33fa9cb4897121b104dd7c852162fa06cf7 in / 
# Sat, 01 Feb 2020 16:40:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:15:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f625aea7552a55d9aac253c9834ea6e645ae1e9d641ccec7e167585699e5d1b3`  
		Last Modified: Sat, 01 Feb 2020 16:45:20 GMT  
		Size: 50.5 MB (50453025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2bd511eb67667a40782667bc3dd7eb41f584de23c5a106085d2a1db980df9`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 7.8 MB (7792989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f4fcee540ca05f3c8904722b70f13e10600fced1073a2612d04d995a93d210`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 10.2 MB (10245802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0daf9041daeed6059c7b11634fdcf512805f7278f0850aed8d6b918609731878
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.3 MB (71337191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eacb949a95d350c4560b4b945e1df5cb1c02b38c8011f930f33659696b843155`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:38:51 GMT
ADD file:a874cf7afdd9718652025bc1f81fdb39341a41d8e4974c1271c6a60c38827dec in / 
# Sat, 01 Feb 2020 16:38:51 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:21:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:21:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:eead0407ee66421148ca3913bacd0ce8efc8ec3454d91b093f8e0c7a840cd526`  
		Last Modified: Sat, 01 Feb 2020 16:43:40 GMT  
		Size: 52.6 MB (52628381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da9f6d041b083f4fba44c0459502c661d52f0df7818ced468ac392766967d09`  
		Last Modified: Sat, 01 Feb 2020 17:41:04 GMT  
		Size: 8.1 MB (8093447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87a6a62880351b6dcbb87be2ef415bdaf2f887b295dab47c80dab8ad5608172`  
		Last Modified: Sat, 01 Feb 2020 17:41:04 GMT  
		Size: 10.6 MB (10615363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de813c0d181da76cd3754f9db008cac716029be94b36afb0e512de8a2dc04621
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74602762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a6f4823ca45daa64dda89e8df04896fa10c4c066a40465c0eaf33a486940e9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:17:00 GMT
ADD file:1a064022bd5caf45345b7a91191b82f0d2bb576e88e99652a4c3d68c399b1578 in / 
# Sat, 01 Feb 2020 17:17:04 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:25:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:26:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c80e92e9d0447b759db73a162ee40f56912d3ae4c251aa735339219ad9bc7a68`  
		Last Modified: Sat, 01 Feb 2020 17:24:16 GMT  
		Size: 55.3 MB (55316324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0367678cef47c5fbcdebd74948fd485de617cb36ea2d6182b1dfd3d5b1429b7f`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 8.4 MB (8352503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc091c35bf183343a79cfcaaa09372d04e69e60e2bf829bb74249782b5c28826`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 10.9 MB (10933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a002226111ff748fe440f194b839c58be9ebc8f8e28cd4c075646c7334200cdc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67867003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d4689befce7bee2f34ccd9e6418edf57fe1dc808f3128f62b467e560d39ca0`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:48 GMT
ADD file:cce6a1a9e391072489b92618430aad507d896a0892b4ab746b46f65aeb50e142 in / 
# Sat, 01 Feb 2020 16:41:50 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:821c3e818de5d8d85868e03fa7647e09cacd5ec4fc251a32c8469652dc6a136f`  
		Last Modified: Sat, 01 Feb 2020 16:45:08 GMT  
		Size: 50.1 MB (50133126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95eab022dfcbfcacdc7e34c79e2393c47272871cba3199d2f185d32eed6346`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 7.6 MB (7592340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fc4d83f881a25a8f4d4dbecfe9212342061b813cb745e8c7fffaa872c5ce04`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 10.1 MB (10141537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
