## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:857cc5251b416b1105b4d1b4d9faaf295e897ed01b447c05ecec0aed824affb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d34c812f68b7964a89e7850a891757b7c471ea95398ef2d7e27df1cb0d274450
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73793751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63bd1a814d6810f02fe1200b850c86355c0102c19a7823ec67fc2d457b29c34`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:21:07 GMT
ADD file:0aaeb8a0c7fde9f030dc2ab67a03f21f44e9eecad9e4cf1f360dc5f768292460 in / 
# Tue, 12 Jul 2022 01:21:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:50:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:51:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4a81bc091a3ce5ccc3c89ef56e710ee1854c5ff9fd3d7f148e87cb956b5b78c7`  
		Last Modified: Tue, 12 Jul 2022 01:26:19 GMT  
		Size: 53.2 MB (53226349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b567a2d645b715cf7eced5f75816db7c980c3416be39e599e6e4b0bbc82f9eb8`  
		Last Modified: Tue, 12 Jul 2022 02:57:17 GMT  
		Size: 9.3 MB (9295637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303c4db152401668239f15446f8107b320fcfdc241030fd93f94783340b469ca`  
		Last Modified: Tue, 12 Jul 2022 02:57:17 GMT  
		Size: 11.3 MB (11271765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9def20650247b2230980ebd69d23330d0a1a30340ee1bcd273342676d3094df9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70694157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68f962fcf1e5b4ab1e32d6070c47a265008661972cb1e41602cd155ff2f9d07`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:53:06 GMT
ADD file:d09e1e4b772f7be41e6f5adcb5a71d86548e6099876e8d5d1bf8eb816a2d8cf9 in / 
# Tue, 12 Jul 2022 00:53:07 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 01:47:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 01:47:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:c8fedff5488db39c94b1a6e628f1dd8a8718a76f0b9f0a65f57e06652448e9f4`  
		Last Modified: Tue, 12 Jul 2022 01:06:36 GMT  
		Size: 51.0 MB (51027952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fdb9c4c566afe6ee79f348756dbd9b7b7752109285ecc12936279d515cc71f`  
		Last Modified: Tue, 12 Jul 2022 02:03:57 GMT  
		Size: 8.7 MB (8725449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece2169f6168d0cd57063262293e9a5e841d140a27a657883596ac7fb3cafeaf`  
		Last Modified: Tue, 12 Jul 2022 02:03:58 GMT  
		Size: 10.9 MB (10940756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9d0c8cc564893f93338da587cbf780ff336be8daa0d06dba5231ae72154e07fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4e650646b48921cfbb93de6480aa7a9514f3836e48d5492c7a794f788fdd7f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:02:35 GMT
ADD file:d11763b9aa59da9e9615c9a7df09de9c36f21a814e568fc0e11405310a9a2562 in / 
# Tue, 12 Jul 2022 01:02:36 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 03:35:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 03:36:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:ce8fe2658d6ff3dea5d2d17cac5d8ea95c2ad6ebd5891a981d88d937403638c1`  
		Last Modified: Tue, 12 Jul 2022 01:15:55 GMT  
		Size: 48.8 MB (48767592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b6262dbfc4ae07e4b7e3e4239774c53b157a42dbd8ffcb7c6e9e122036e7d`  
		Last Modified: Tue, 12 Jul 2022 03:56:08 GMT  
		Size: 8.4 MB (8405583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a757a2ad0986080b4acea992995782caa9151b4dcfd8acecc382d0bf2ae7e33a`  
		Last Modified: Tue, 12 Jul 2022 03:56:09 GMT  
		Size: 10.6 MB (10585915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b938bc2c9abf52f196477963146f37d259cead2e226d80950483167e4bd66497
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72528212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c932177d42941c6fda777d16de5930c0f4d5b5a24eb40c0c2d3b27344ed189b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:40 GMT
ADD file:0f18dcfe7e502abae9dd7f72911dda640e4675306760d63f467092f962228ad1 in / 
# Tue, 12 Jul 2022 00:41:41 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:36:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:36:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d3ef27d3c918a6321957a64c33268d09a01ec18590cce79a144625d9c0c8599a`  
		Last Modified: Tue, 12 Jul 2022 00:48:17 GMT  
		Size: 52.3 MB (52331756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f3b169736466d16aa015562be48cd38804707291d997ad0a77f69293eb28a6`  
		Last Modified: Tue, 12 Jul 2022 02:44:53 GMT  
		Size: 9.1 MB (9139825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fef5554fb71c819accf1cb6b60a439cb9c6a8da7ad329ecdfa59582ef1f116b`  
		Last Modified: Tue, 12 Jul 2022 02:44:53 GMT  
		Size: 11.1 MB (11056631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:185f59f60182bcefff6b67591257885f87b042f4c3922e7cd2912e2940be7e85
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75143696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa39c872e318695e9dab3882eaea5e844e97b2487307753561f227c4d79da48e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:33 GMT
ADD file:f76df7d0d2c0977290a0183cbc4f62656ab20d04eb0cae4d075fd31ddf9df8b4 in / 
# Tue, 12 Jul 2022 00:40:34 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:30:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:31:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b7f5437d02adf5c6ebc8b31ebf7b4950c58003a838e1f6591ce754472a3bae43`  
		Last Modified: Tue, 12 Jul 2022 00:47:20 GMT  
		Size: 54.2 MB (54207595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd45fde68a9a7357df097d16053cd6c09bd1e8e11d9a007f639e8450c6debc88`  
		Last Modified: Tue, 12 Jul 2022 04:38:27 GMT  
		Size: 9.5 MB (9466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb688f237713e90f9618c949c97ebc2f9695bef669becebbfac33581372c6f5e`  
		Last Modified: Tue, 12 Jul 2022 04:38:27 GMT  
		Size: 11.5 MB (11469728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:43e16309cb69f315fa86449937b420a80740c59ce60c263656a94d8f08232b92
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72044413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea28265acbcd742b4955516d063ff0dfcac5c8b9c6156eb7fa5bea60e53cd7e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 04:44:00 GMT
ADD file:f6825f1dd59126d26ef0dba330a1d0eff37f6b9d56fe4a1bf2669774a6a7c74b in / 
# Tue, 12 Jul 2022 04:44:06 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 06:27:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 06:28:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:043042ab5eb51d2e5fe9f7bf85b86a91823ebf404e02b09bd9d96e29066acc7b`  
		Last Modified: Tue, 12 Jul 2022 04:54:59 GMT  
		Size: 52.3 MB (52346196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78102f519b643046757a9cd4f6d008518ddaf7e24f82322dba5336a7bff1dd7a`  
		Last Modified: Tue, 12 Jul 2022 06:46:55 GMT  
		Size: 8.7 MB (8664834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3efe7ae97a67b5d9d9a2fd74d9d6407dc893ffcf6df03128e98d57bb34138`  
		Last Modified: Tue, 12 Jul 2022 06:46:55 GMT  
		Size: 11.0 MB (11033383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5935aeb9227e6a4a1d2ce6229094ff5b280bbaab27e0c39610bb6725e46d8cbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79413982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8b58cafdbe6f780fa3a3fd1027197af4abf570997f33303bb5db5158be93e1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:27:28 GMT
ADD file:8039654bddce2cd83d9433d1df0a53c329e7877cc8210593bcde23de63e2f1fd in / 
# Tue, 12 Jul 2022 01:27:36 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:49:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:49:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:0d4394941206b4f218ffa2a2b794698da5149ab7a22b52f71390aec65a7add3e`  
		Last Modified: Tue, 12 Jul 2022 01:40:47 GMT  
		Size: 57.4 MB (57441462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e13dc094f3be3cdae228630277f198c2aee4ccf4989e03df692829782575ad`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 9.9 MB (9889588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9148c549699d52333ba063274d8397af520c8317b8d893c23ba0800047eb2b45`  
		Last Modified: Tue, 26 Jul 2022 23:51:25 GMT  
		Size: 12.1 MB (12082932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f3001e6db8ff5ae74e465a953fb9a1d3dd64846bbb31f0d42fe5493b1b59f92b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68491637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7648e9385ddf020464c24f07cef291a6853a4552ca65a6b8e8253e26708443a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:10:39 GMT
ADD file:bd8475470f5c6f95d31c06b918cd7725db4098699597cddbe66f7d30cecdebf6 in / 
# Tue, 12 Jul 2022 01:10:42 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:16:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:18:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:e08ecdb135d5f5e0335332e1597ae44e5c8eb292461b299517cd917fed413256`  
		Last Modified: Tue, 12 Jul 2022 01:28:55 GMT  
		Size: 49.4 MB (49440738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb7bba79828c7c077abda404edadc49cf674ae2d2268ef7749779a9b29a75ce`  
		Last Modified: Tue, 12 Jul 2022 02:59:04 GMT  
		Size: 8.4 MB (8394915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e028c389ce83680914e57b7f8fa251005e8f6822edcc336e7d10417e63e80fbe`  
		Last Modified: Tue, 12 Jul 2022 02:59:04 GMT  
		Size: 10.7 MB (10655984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:62699f36e296ebf4c43cbb6b2af63874698e02388c914239c012320b78470bdc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71859543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2355d79e2f3fc2f5009bf9c18c05bf8b2f8ecf2e2b0078c1fd7b711ca9e13132`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 00:46:07 GMT
ADD file:160fd6ac1dd96abed2e1719ac95e75e8a8eeaeef9e04a353e0ba4a23cbd1c1e4 in / 
# Tue, 12 Jul 2022 00:46:14 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 02:45:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a4ac3f896d9c36c21fdbee9a7ab2637136d4d09ef6db30c3b2b4ab10c48abbe7`  
		Last Modified: Tue, 12 Jul 2022 00:55:11 GMT  
		Size: 51.8 MB (51757401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7d0c4835633a8b04da06d28abb8af4b5557ef25b136337b6872fd92b710b70`  
		Last Modified: Tue, 12 Jul 2022 02:55:25 GMT  
		Size: 8.9 MB (8939218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deabdcf7f5d4d109945eb55d7a1fda36ddcf55c65eaff794d0456ee0e0e2e30f`  
		Last Modified: Tue, 12 Jul 2022 02:55:25 GMT  
		Size: 11.2 MB (11162924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
