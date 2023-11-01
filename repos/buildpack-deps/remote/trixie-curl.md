## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:6802227530ab171148a4617723d51e3f70801e7489447bbd91b4354d37fa526c
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

### `buildpack-deps:trixie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0a83183f7c37c53a706b095ca3f476a1c685cdfae41ad49667eaa6453d3ac3fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69812643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6248e338704ed0103a72cedf26cec4ec90af9944acd6776e9c5dfd2d07a31e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fc83c09b27b5464dc8ea8a5446245ac976b0539327658f64cf6f92fb6bcd3f`  
		Last Modified: Wed, 01 Nov 2023 01:06:11 GMT  
		Size: 20.3 MB (20325758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:028a1c9e692341c831163d6b76ec37278dda15b1a352d015bab413b4a755ff82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66533670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0bd68aaee20326384cebfe2192800057c7e52b8759c97f482b4e603d88026a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:02:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a39eb0fbbdbde2ffc32c0b9d238b1b619908941738a46e434466685cb4012c`  
		Last Modified: Wed, 01 Nov 2023 03:08:20 GMT  
		Size: 19.4 MB (19391553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c5fc1bd5425c90d682eef8c7af83a01cc8b6e760fe2256bd6aa0f58525a77d47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63600002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe71bb45453eaa504b31498a37608aa4276f044bdd18560a39e673d93b2a243`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:38:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec8c0ca01c5e4b512593b2689b47c59c49816c34e108183c62760e73fdd443e`  
		Last Modified: Wed, 01 Nov 2023 02:46:03 GMT  
		Size: 18.7 MB (18663805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5c597fc3f240d9ec58bc7a8bb6eac544d7f91bc95c583c0dea4a8c5343d2cd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69636607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799b9d80cfbf3d254cc2d8e1ba2618aeab9932ba566919d1c5b40598e8817518`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:805dd0cb6d20f9293082e2731dee26c4189ba2e05e33a9f191a996164477f318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71372123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b67991ebfd3a67bfb234e83a7242703653494aeefd5471beb24c4e239b52a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f51f1238b9640b9e5ee718926672d0df20e00b0acbf2c2b311248148673bbc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68895374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db4384cd0f6fbbde63af84a9a7aba48e7ca88a8045c743733eb4c43414eed70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:69498a6f72a3a01ea0524aac08e417b193e22fc14a455000e6cbca7b42d355c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75057087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1e802f055f46349722e6593efb91dae34787edd86e823058f2d9649da2fda3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:36:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6abc26e480b6b4defaea0da8429302a281509813276f95bd58dd3fae6a5e8c`  
		Last Modified: Wed, 01 Nov 2023 01:44:16 GMT  
		Size: 21.7 MB (21666389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69f5a6be863cb69c5e8fbf9fb8eaf91c2994ca992b4db4df61c766a3dc512c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68959952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c167457a1683a82fde1556d548ac9344db2d2d3e22530763b33801be31261264`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
