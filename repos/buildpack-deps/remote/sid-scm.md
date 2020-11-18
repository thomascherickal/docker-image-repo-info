## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:6b955d4bdd2dcf1a59b4ea31e483dc0ce60cb5b7a07818847e01ba783262022e
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fb28905646673ebf2a4ecfe0e0ce64623a21e39d26fd6dc948724067fd4b7d88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125443500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06ec22e747b171d4071bb66d9fef2ff80beb9449dd7f8dda1408c04b1cd1e164`
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
# Wed, 18 Nov 2020 00:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:ae65daff77b5d6ac0619bc955c2b1edd6ad35d46f9ad26b02f3de5bcd0951da7`  
		Last Modified: Wed, 18 Nov 2020 00:52:58 GMT  
		Size: 53.8 MB (53755325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:62a2e5d6ab8cb8a94a0babf52407e1b718f6ff1adcce35a45424d5948c065fec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120352568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d2139b7aa626afb86723983a0ba159e5a4a5548d16cdc76d11e9941f6a274e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:25 GMT
ADD file:48fdddee7022ba5a0519e9f9dc9a63dd483e5294d0cfed9db93b066547405eec in / 
# Tue, 17 Nov 2020 20:23:27 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:54:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:55:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a5730ec2f66f57a119aa59f80f288eee4fa0a1adebe48e9a184400d277b84ee2`  
		Last Modified: Tue, 17 Nov 2020 20:33:13 GMT  
		Size: 53.5 MB (53546003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7216d292993333f9d256b5efb205324811bb27a35f161c01af5690ebc3c5dd10`  
		Last Modified: Tue, 17 Nov 2020 22:11:18 GMT  
		Size: 5.0 MB (4974955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97e0fda183c339defd615cf109c141a20426f4d5020d3d97bff391567c03d72`  
		Last Modified: Tue, 17 Nov 2020 22:11:18 GMT  
		Size: 10.3 MB (10332185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d725a7f9c1177aabadd58343e4662e541fe14a80a7e2aba6fe018f23b442c`  
		Last Modified: Tue, 17 Nov 2020 22:11:45 GMT  
		Size: 51.5 MB (51499425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:21b04a00eb75d4c32b7aa10370d45fb2437680ae9cb6d93ea7d6a6bd7851f884
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115433419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:778cb54381a5d24e5744e2eb0211890060d51f5bf6067f7aee4556ce0b700987`
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
# Tue, 17 Nov 2020 21:53:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:84fe46831ed801ac2a919749edc60b1551dfa37d991390ce0b16b36fcca04a6f`  
		Last Modified: Tue, 17 Nov 2020 22:10:29 GMT  
		Size: 49.5 MB (49497168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:87dcbbc1985d24d4e1add2f58d37dcae06346cb616d0f1b57eff4da715375f44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124280863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a033e73af49dde4414a9fe7d63118a4cbf46f28dd17ae862af7c6f6f3893a65a`
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
# Tue, 17 Nov 2020 22:25:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:1ffef1fd67608c1c75fe7d564719a6e2a098fe43f43dfddc1dac311b1fccbd61`  
		Last Modified: Tue, 17 Nov 2020 22:38:34 GMT  
		Size: 53.9 MB (53856622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:f74a7cd774a9079bdc7a45e46092cf8ded582cc8c1b487dc516f2ff982cf931e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.4 MB (128376510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4526af7986e498c2f897a3baad7d300fa1e59fafcbc6d67e9d3015df16d0060`
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
# Tue, 17 Nov 2020 21:17:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:c97dd1237dfa1a40c9c2255e2dcdec27f7d739925bf6b97716b25759ca483baf`  
		Last Modified: Tue, 17 Nov 2020 21:26:43 GMT  
		Size: 55.1 MB (55068291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ad536501efe3f968ac67517c62c164c79f86bcbf986772a27952e4cd488439a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122520043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72b43698665339ce1729d8660173c7a7eb37c4ea91face703d765f1a7f96e18f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:54 GMT
ADD file:e6702c456d50f8685a251f68c8f1ef26036f57dc2b0b3ee32a713a0fff6192eb in / 
# Tue, 17 Nov 2020 20:19:55 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:44:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:44:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:45:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:15e7eab80614971302cc43d79249de4c2eaedd05f7ae229c90002e6998c37745`  
		Last Modified: Tue, 17 Nov 2020 20:27:23 GMT  
		Size: 54.2 MB (54247133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb52b20dfb96ec0abe6e94d1493602c96b8050c535a911f580f3723be5bd3b7`  
		Last Modified: Tue, 17 Nov 2020 22:55:28 GMT  
		Size: 5.0 MB (5026356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe047368d6844c3bab8d888c6322017279e7a1ab2f8537217ab3e70de38f39d4`  
		Last Modified: Tue, 17 Nov 2020 22:55:31 GMT  
		Size: 10.7 MB (10652949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d6065e8232fefa2254da6923065a6ed63fedf4ac24ab6065b69e66160d7d9b`  
		Last Modified: Tue, 17 Nov 2020 22:56:22 GMT  
		Size: 52.6 MB (52593605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:481ab70cab70e48cd98e4d4d98597e1b924d466e0d76f3efae514429cf9a4de2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140947145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537c7cb938d258ba2d0abaee1743d13aacf0e6c732804ea5809693e4234b35b7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:24 GMT
ADD file:7998a5d3f49a86501eb252e7dc54464d086e8239a5f918b15cd85dd11e7341bb in / 
# Tue, 13 Oct 2020 01:39:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 09:10:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 09:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 09:12:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ab405c79eb283d457b4f978511bbef215699b366c926b3450f2a7cbc6a56e33b`  
		Last Modified: Tue, 13 Oct 2020 01:51:11 GMT  
		Size: 56.5 MB (56495338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38962ab4f4d37e5644006dc2c9a5a9b270448a5ea5ea29a387f4c7955497875d`  
		Last Modified: Tue, 13 Oct 2020 09:38:29 GMT  
		Size: 8.3 MB (8329668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8ecae68ecea0d3add456e8b38f9eef46b95731e6dfca00f430a45a774f2a19`  
		Last Modified: Tue, 13 Oct 2020 09:38:30 GMT  
		Size: 11.4 MB (11392727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfde9fce3dd7addbd894e0669be922a792dc5fa95b3ee33ffbaad4ac26cb393`  
		Last Modified: Tue, 13 Oct 2020 09:39:33 GMT  
		Size: 64.7 MB (64729412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3a2b0034e6e556c36a37f0978e0e826fdf6145b354954fcd20f1cfa2cc544b90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123009084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5cf2bf148028ed9fd87d2e4525dd2dfef0a5a39eae2b4ad21ca92aecf24cb3`
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
# Tue, 17 Nov 2020 21:37:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
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
	-	`sha256:b358c5f7f1a0229f7d7aec3a9cdf564e0198552849099d872ef5cd94e80b63ed`  
		Last Modified: Tue, 17 Nov 2020 21:56:08 GMT  
		Size: 53.2 MB (53231631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
