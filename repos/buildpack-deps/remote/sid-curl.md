## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:6b98723a6d160fbeb2f839fbaec60cbcfae4a0f414c0535bb7b31cad1697552e
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0cdf8fc2338e2908aae0b8cb9261f56e50595167285a072468eb878f56b54fff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73322397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a98fbb10debdd5ff695d7f1d1c74300723c33abc60ed5431de34067fcb9b2d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abee259a1d9101a0890f49e244222094315b4c017c58d8cb8a6cc0cd43e833`  
		Last Modified: Tue, 13 Sep 2022 03:52:28 GMT  
		Size: 9.3 MB (9298049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8698192cb686ddacc8322753abf5c95c28d7cca2e06243ec755c2044f89760`  
		Last Modified: Tue, 13 Sep 2022 03:52:27 GMT  
		Size: 11.4 MB (11380792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6d4954538c468e745a487851cb44a6cceee8be373e805c22bd384678992c8a39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72339574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5de3670778fe98accb2c7d82cff835e13b367e2d981e9b6d033403159e07eec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:23 GMT
ADD file:5da40917ed11781002a72811aeac4336d50b3100f4e25213b5b18cb733468d31 in / 
# Tue, 04 Oct 2022 23:49:24 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:19:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:19:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f013d31fa02ab56c7186e21477e4fd559e7e9de70eb511ed30a523990b759421`  
		Last Modified: Tue, 04 Oct 2022 23:54:20 GMT  
		Size: 51.6 MB (51568969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f385ca45e727337dc6e057766a57c9badc26c5e75234bf0aae01ff5692ac8674`  
		Last Modified: Wed, 05 Oct 2022 00:25:04 GMT  
		Size: 9.7 MB (9739988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b50d6779e58a2088ad2ca98253c952ea1e71f4dd19953b82651ee27cd45794`  
		Last Modified: Wed, 05 Oct 2022 00:25:04 GMT  
		Size: 11.0 MB (11030617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:875f7ad20ada13262b8bca84b972e32a989ce37fdd33d370d3bffa7a0b0d9215
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68580647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d763e51c5b076bb7e7e9b79225a4c76eaa410e1ebc5c7116b74f21c232139129`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:44:03 GMT
ADD file:6c202b99cd5c91b3c2b2bc39ddaf5738d4def8520e18a716d249d62881657e5e in / 
# Tue, 13 Sep 2022 03:44:03 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:261cac8f52f598a2e1428463187e026d01259f7076e6ca3adf9b13c1414ba47c`  
		Last Modified: Tue, 13 Sep 2022 03:52:11 GMT  
		Size: 49.5 MB (49523940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e346b65163965ce437753259a3a5635ac1fdc3d48b6735d5be0f1dc103653`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 8.4 MB (8397051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c75620166463dd3a4557387e6591fccb3f2196f7d3af1c7d033dd15cc6cc0cd`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 10.7 MB (10659656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb882756c173baef892ec51efb1bb17e70987a2cff7c18c9dc294a3fdeff9d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73364877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:350c353bb13622add2ff842bab87cca0ae1b5fd93a0ebf6bdec67db797c3489d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:54 GMT
ADD file:13af7384e2c4f0c81e2c22e39e5d930dc4524d300c5f3d92ab3288096c308777 in / 
# Tue, 13 Sep 2022 02:11:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:04:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:04:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:113c8010a5d8650dba62a6df118557cb9b270a562e4a0537563cf79291f65ab0`  
		Last Modified: Tue, 13 Sep 2022 02:18:11 GMT  
		Size: 53.1 MB (53103634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f00ceb8508161cf15d9580001f11e56a6e5eb7d0293d831a4d3bb4932e1050`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 9.1 MB (9127731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac595041e810cadc49116d5630a0f49b2e0bb6084756143d92c87a24e9c24f`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 11.1 MB (11133512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b5b9cce12f09fe605dfcb09f6fe8500023702df50163f827ef19bc9038b7fd5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74701692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b40f92cafe5909bfee9b18a6b30b1f595e047ddead64f49c8681bb408ffaac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:40:48 GMT
ADD file:ea6d247c762f6294c87144d1a4308c30669e9e732bd8ff9ef892c71d14563165 in / 
# Tue, 04 Oct 2022 23:40:49 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:12:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:8a0d07a7940ebb4ded014cd2eaedc6b9aa8767ff5afeee7b1b09fce7cbd7a31e`  
		Last Modified: Tue, 04 Oct 2022 23:47:29 GMT  
		Size: 53.6 MB (53647464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9d75da7404fd11d9c4d9f1cfda7e84d06616c2862585b352ba3d0cb4fd437`  
		Last Modified: Wed, 05 Oct 2022 00:24:14 GMT  
		Size: 9.5 MB (9475965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e558ef32d8acfcaa5f0d607d533c5b5febbb588f2a71986dc1bab69c9a091e65`  
		Last Modified: Wed, 05 Oct 2022 00:24:14 GMT  
		Size: 11.6 MB (11578263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:569464ecaa8e532d06a96a80c75fc9566c65fcfef99e33ad9bde7ce0c97d67a0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72868421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe44fce6a7503ff70aa5e19f32c0daffd778243e3b2135bc88a2819019d5724`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:30 GMT
ADD file:dc60ee74dfccba12269b444dd45f20e0133d724b1942c6b0f9c5194eb68bc303 in / 
# Tue, 13 Sep 2022 01:11:36 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:b00b55b6e19db9300c81bc3c7da4bdd60a1432296143ff24c14dc6d0eee819a2`  
		Last Modified: Tue, 13 Sep 2022 01:19:36 GMT  
		Size: 53.1 MB (53078760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86798e592e4c27c8b93559a482630aeb78e21c77d475b6073a710cedc010c221`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 8.7 MB (8662682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e754dd24f2e4a96086e83f849cac69c8b471a4e9c281073faa059f3ffbe46df0`  
		Last Modified: Tue, 13 Sep 2022 02:09:03 GMT  
		Size: 11.1 MB (11126979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f0fd4ab9d4da3b6fa3a8000cb9481cf35e68b38ff3471abe82967ab413c3d9b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78816852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df175a7c6922a086c362aa53ec99b3cc113f66535939a6fae9ae4b4bb482c030`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:23 GMT
ADD file:9a1fd28de3c910076975890aa736e3f3bbff1b433c668f4121cf52af264cd06b in / 
# Tue, 04 Oct 2022 23:18:26 GMT
CMD ["bash"]
# Tue, 04 Oct 2022 23:56:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Oct 2022 23:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a99fd400e2fbb8830bde6fd270def7df44ad1a841ec4e7cb5f33d7f5661d181a`  
		Last Modified: Tue, 04 Oct 2022 23:24:45 GMT  
		Size: 56.8 MB (56786765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182d06bb7b49d3eb3a82cbdff85d58cb0731d3d80785b0934f25001bf5bd3fbf`  
		Last Modified: Wed, 05 Oct 2022 00:06:08 GMT  
		Size: 9.9 MB (9885071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e5e780a2b80f3c4caf46c625dd63314a82efa8edc7f5d9d6442a7edb4905aa`  
		Last Modified: Wed, 05 Oct 2022 00:06:08 GMT  
		Size: 12.1 MB (12145016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4a2fb00746c69ff675e9a4b7c33ca1d49bc7876081e0d523d3d5c0369ce1d8c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69105062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d5b08235820d175371883da59a21eef0884d079863088dc9f96c4b6e759832`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:31ea8864ee36fe749530f5fa2d599d61820e8d38ce13dc1bf7121f74b4f5fe02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71711809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a8d1b3e3f918c33cd486c119b5c2746c20d4da7e5c6a3366af0ecb178aa714`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:19 GMT
ADD file:c95e2b098d871c8f60e72d16096a4bcce80e256166b62df3ac0abf8c1cc5384d in / 
# Tue, 13 Sep 2022 00:48:22 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:27:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:27:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a47738c5650c377467230bf819bb4be695718c6effbf5489b6e0fc8e11229d95`  
		Last Modified: Tue, 13 Sep 2022 00:52:55 GMT  
		Size: 51.5 MB (51537006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92aa5a30de3637ebbcd271e1f1795c92f2432d80f355e866dbb37a7875ba82d9`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 8.9 MB (8935914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2c639682b677cbe7eebdb0376ad10594f99f1d23baa05fe3c38f108872567c`  
		Last Modified: Tue, 13 Sep 2022 01:33:40 GMT  
		Size: 11.2 MB (11238889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
