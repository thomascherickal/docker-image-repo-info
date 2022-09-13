## `debian:experimental`

```console
$ docker pull debian@sha256:23eab9184f8ac44e4132b21698ebebd3d1f85e4a87f11a7cce4320a65f7bbe68
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

### `debian:experimental` - linux; amd64

```console
$ docker pull debian@sha256:b543cd094edd0c9271c9b5fca680344af2fc418a057b0d63276b7e07cfa744f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52643827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8726d4a11d5a96a53b643c2295a1091d3ab5e77655e107f20885a1950835405a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:58:12 GMT
ADD file:6ddd5244833a0a8b71e79b85b68064bd5b09f430b1b0ed8db07d6855ad470c39 in / 
# Tue, 13 Sep 2022 00:58:12 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:58:23 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:d48fb30607a31176a332991b7110d4b196c3564594e7aab632b9662094ec885a`  
		Last Modified: Tue, 13 Sep 2022 01:03:54 GMT  
		Size: 52.6 MB (52643603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feed5ae45c9f1637fd673679cd602a43eda6d5645f8656d5220cb52bd1cd905`  
		Last Modified: Tue, 13 Sep 2022 01:04:17 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v5

```console
$ docker pull debian@sha256:92cef5e5007a0834e3ff2301cad38e5fa5ffaa802f02bd29642f4170f15d3b66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51786153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89292022e7fa88d2015b754dd03457cbe7a8b265b040d276bc7042b5b32623eb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:16 GMT
ADD file:e7ec9bef12457f73465a8b9b0d10d2ee3fdcf244d19625f58ba4ffc2fcab0a1d in / 
# Tue, 13 Sep 2022 00:56:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:56:42 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:2ea2e84f45a0dfa7c04aa60a28b638e9696ca74b5f08fff59842aa2fadadbc5e`  
		Last Modified: Tue, 13 Sep 2022 01:04:36 GMT  
		Size: 51.8 MB (51785933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e1d1040164c9b35fe18a10cf8b6b71419e3fad3fb828ca0d3e407b584c0818`  
		Last Modified: Tue, 13 Sep 2022 01:05:10 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm variant v7

```console
$ docker pull debian@sha256:774ab6ddc9c24482c6cb196db623b72ff872c32c54efa9508738d29b7bf06262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49637664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:818803a968149ac7c64e2b9446840823754e9c207c9122ed4162177e5620ecaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:46:07 GMT
ADD file:9c91d918ee9751534cac81195704988dee25885035e80050be846366deed315e in / 
# Tue, 23 Aug 2022 01:46:07 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:46:23 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:b86df858a415c9e0122fe7bc076cd4ab39d4874a294bf82ea48acf9f2e8bdec9`  
		Last Modified: Tue, 23 Aug 2022 01:54:18 GMT  
		Size: 49.6 MB (49637444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4ce24ce6603fe76177746d7d7bdaf32d4a5a7e3c9ffe8506654514b21fe683`  
		Last Modified: Tue, 23 Aug 2022 01:54:44 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; arm64 variant v8

```console
$ docker pull debian@sha256:5ee68bdf0eca46eed53116147be4d64aa75f0ab0636d3507107598e9d865459d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53220857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a3676bee7ba5efa3b9f3455b5d68e32695a0b79d338b9104de6a06e71a82fc0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:54:40 GMT
ADD file:e25df43e28798ae6a4983fc5503d82e8f9cfa5b9ec82a1089e3f5ed71b5556d7 in / 
# Tue, 23 Aug 2022 01:54:41 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:54:56 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:dc70e2fc176f182fa1deeacf225b6cd8428bc0eb0126f14c56c4be54a2d4021a`  
		Last Modified: Tue, 23 Aug 2022 02:01:43 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3156bee05531b9ac912e1138e576d2aca4aec5542d35640c258e86838ef2f7`  
		Last Modified: Tue, 23 Aug 2022 02:02:09 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; 386

```console
$ docker pull debian@sha256:ad1d7d191c45265ea94cb312c58f340f7d0d94005a29e87e022dbde05ad63926
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.1 MB (54133937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0964685aab45ac96fb105ab0bb4def63da7ebf0311448d3686dfabe9671199e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:04:53 GMT
ADD file:afdff393ba92147f6e5feea24b8953956ffe40bb737905ad5887fdc3bd1cc45b in / 
# Tue, 23 Aug 2022 01:04:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:05:09 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:3f7095fe316e7888814f4c75a3ebbbae200024e40ff42ad69770862f99e58b93`  
		Last Modified: Tue, 23 Aug 2022 01:12:29 GMT  
		Size: 54.1 MB (54133716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a4aa0c86e4f8c5791c388a8f3c83abb0a5cf7d450a44e05e888a772170a93e`  
		Last Modified: Tue, 23 Aug 2022 01:12:58 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; mips64le

```console
$ docker pull debian@sha256:7f1b884cbbffa5b3e0d22f887d427dbf8f9b7f7bae3e4085dd5aee0a0baab28b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53216875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7054f25de1425f072e88a81807a07f1e3f38fc2072c6807c4dd3a120cb230e4c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:27 GMT
ADD file:289ff967122b94852c18b08616d72bff729cc9d607c295c6c758bb8917ce5864 in / 
# Tue, 23 Aug 2022 00:15:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:16:13 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:10ecab1bdcec7f490bd4865c91fc25cfc0d3d5506b9673055d7740a86765bdea`  
		Last Modified: Tue, 23 Aug 2022 00:24:06 GMT  
		Size: 53.2 MB (53216652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8187526258e55e7a283249775de7fdac990d25e667fd1d930ae0538e05ef8d`  
		Last Modified: Tue, 23 Aug 2022 00:24:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; ppc64le

```console
$ docker pull debian@sha256:55e464f3908c873bf8f3dc4ff6de372b7eb95e85b5b839b9448cf0a4e93a87a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57314109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4359dc8904b93ae0cc8eb615490b24e650573854ee066e0964a0accc5494238`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:26:59 GMT
ADD file:e0a304b32aeec78fd97b6a5d5b40507c82f92fd0090fb2d6e097d09579468800 in / 
# Tue, 23 Aug 2022 01:27:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:27:22 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:26694295996e09ba28755431392df314dc6f483328a0e25462fd720fdcad2e40`  
		Last Modified: Tue, 23 Aug 2022 01:33:38 GMT  
		Size: 57.3 MB (57313888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aed66c91fa7715d2d443da572622d4a06dd2928caf0f0241d4be68cd2f7cc`  
		Last Modified: Tue, 23 Aug 2022 01:34:11 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; riscv64

```console
$ docker pull debian@sha256:d0fc011bc400eec92d94f1fd20be03a0b297fda36f5c500670e6a3fc607ce352
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49268422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b818a232cb48bdf3ca4b84bf371194cf9db7306df1a847f76a5b93c975490ee`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:15:54 GMT
ADD file:922879b545740da41d47ffaf3bb1d9f5cae855386457ae213834f5f1eb869dac in / 
# Tue, 23 Aug 2022 00:15:57 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:19:28 GMT
RUN echo 'deb http://deb.debian.org/debian-ports experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:243eeed5cf29613bd014532fa4bc8fb367b678d2973dc4a950c09bd2df4886c1`  
		Last Modified: Tue, 23 Aug 2022 00:34:23 GMT  
		Size: 49.3 MB (49268194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9074adb383b955e8e4e755127062849db72c1e821950bf6386d8470eff567f`  
		Last Modified: Tue, 23 Aug 2022 00:37:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `debian:experimental` - linux; s390x

```console
$ docker pull debian@sha256:5be8b87514dd868479dc2731fda809a9f08f777df173fcb0af703500e4eb3f5c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51537223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f517eb61c1d8e9b97f0c76d87e074b3f23f21666d093fd138daffee9db97d66b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:49:41 GMT
ADD file:218a929c0b84eeef4dd935bbc23ec1a4c9fc02f06cf5c86ca6c8e94e78c5f927 in / 
# Tue, 13 Sep 2022 00:49:44 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 00:50:04 GMT
RUN echo 'deb http://deb.debian.org/debian experimental main' > /etc/apt/sources.list.d/experimental.list
```

-	Layers:
	-	`sha256:ee6e329c518cbd235ab8d38fbd5ffb98ffe45bfb2874fa69e7084eb6ecd09ca1`  
		Last Modified: Tue, 13 Sep 2022 00:54:17 GMT  
		Size: 51.5 MB (51537001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e60677fa0219710676fe7d6c382b68d19f4d901be63afc7e617ba536f3dea5`  
		Last Modified: Tue, 13 Sep 2022 00:54:34 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
