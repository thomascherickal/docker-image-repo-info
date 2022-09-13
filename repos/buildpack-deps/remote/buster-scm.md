## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:07e999f2b4c56d4a9e8e5be86f2e2d865c22e6786e0322f7316bef4a3f65765f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6e0bcb5f43e3716650504bd865fb97b8e716862019548c5b8181fa46a46e6c96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.1 MB (120139810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d224791ee3e77a22ff9032970ebd89675d352cf03457d4853f43f4aa05c65cc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:38 GMT
ADD file:4649a893b2859f2ff51182a13c9c8eeaeaea866161b3f4a1c4f0bb48bc01d007 in / 
# Tue, 13 Sep 2022 00:56:38 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:44:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:45:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86467c57892b6bb48d563cb5940c68b69c431b2e79c3547df60d1c761c21c156`  
		Last Modified: Tue, 13 Sep 2022 01:00:51 GMT  
		Size: 50.4 MB (50440374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b34aaa3cba7676359d4f9d29333c92bd9f448969b07f56bb8482398a5dc53c6`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 7.9 MB (7857266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a443ab54eaa5455912b469fb6d8b621ade658cd0afef9c706b7e37085004b25`  
		Last Modified: Tue, 13 Sep 2022 03:51:20 GMT  
		Size: 10.0 MB (9998148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cacf42b5677aa20eb8fff5102f7482828f27555a167f49da0597869f91002f`  
		Last Modified: Tue, 13 Sep 2022 03:51:39 GMT  
		Size: 51.8 MB (51844022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2b21b7e68297045f0648ee6c7a3a7cded66b6942bb212597f001c93b6b9089b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109767207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205ee4a6e0360d9d5c60333ba1ed2cbe28c5f07385f68bb62198006f6261bba4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:55 GMT
ADD file:28e8fbd48a4aa7f5294aa6046899d5d5cbbd70ba28f7c6d3570d4f92dab36103 in / 
# Tue, 13 Sep 2022 03:42:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:33:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:34:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 07:34:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:03c0a108fceb58ca60977e45057eccb02892db7412dc4da52f05ebeacf68951d`  
		Last Modified: Tue, 13 Sep 2022 03:50:16 GMT  
		Size: 45.9 MB (45914887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8d9dfb719c68b4e85536bf44f1f2f7abda57f49fb9db0aab127aa94fea736e`  
		Last Modified: Tue, 13 Sep 2022 07:45:37 GMT  
		Size: 7.1 MB (7145364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbac34bee21317dd05d321de4c580f6de3f0d3bc156a2b8fb29af4a69bf2b96`  
		Last Modified: Tue, 13 Sep 2022 07:45:37 GMT  
		Size: 9.3 MB (9344332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddea39d4af9713155087ad2ccecd0a8ac864c2a41d4acda5cbfd8bc7e954759`  
		Last Modified: Tue, 13 Sep 2022 07:46:02 GMT  
		Size: 47.4 MB (47362624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2b90ff6a63c2884d9ad9197f30bd260a0a0b658c77d35b42da550e7f63f56786
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118894562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e1ddd021f79d6d3d45ff42d9b5e4811ff24162e9c03592e4bd840e62576044`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:06 GMT
ADD file:304a544562f139d7ab96511b7f1e059966cf90169117e835072f132468bf91c8 in / 
# Tue, 13 Sep 2022 02:11:07 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:03:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:03:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:03:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e2406a452ad23ba9085e0708f5e15309206a618eb828aa307becbb239414392f`  
		Last Modified: Tue, 13 Sep 2022 02:16:42 GMT  
		Size: 49.2 MB (49228261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91678e90eed09f0ef020521348ac09d6816bafc59c40f4fa0d821de2fb50f881`  
		Last Modified: Tue, 13 Sep 2022 05:11:16 GMT  
		Size: 7.7 MB (7722146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d9f7a2d689202901c1750505adb5481f0e4499998084e1df70209fa11f8e8b5`  
		Last Modified: Tue, 13 Sep 2022 05:11:16 GMT  
		Size: 9.8 MB (9768786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e42f230da3003e92b349e81764d6c82232541223fa1b17d44222328b0cf201`  
		Last Modified: Tue, 13 Sep 2022 05:11:35 GMT  
		Size: 52.2 MB (52175369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a73aa30640092005bc7e3c9ae4af03341fe9b48f482b6bb50f52ae12f201ed02
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122797838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1eab58bc01c9b14e0d169f5be848832a259d48915636e62e131a622c8a7985a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:56 GMT
ADD file:abd47beae46939f6ebc8cc566b1f23f170bd1b9318b1ef10dd16ea4209140bd0 in / 
# Tue, 13 Sep 2022 01:39:57 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 04:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a0702c36e95be838f5e174ceb286969e8527f17111141f2c8a8ecda44d0a14d4`  
		Last Modified: Tue, 13 Sep 2022 01:45:44 GMT  
		Size: 51.2 MB (51202973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be8b5f305f5479b300e03b1ee4b19b0008833df2d269be3dcb6caff4e790abb`  
		Last Modified: Tue, 13 Sep 2022 04:58:21 GMT  
		Size: 8.0 MB (8024065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2875198ef388281cfb712c18bf183cea7a0597a6b05b7894e9e91d2a585e1d`  
		Last Modified: Tue, 13 Sep 2022 04:58:21 GMT  
		Size: 10.1 MB (10123769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19d1325da1b59cc6eae7d3e5a5bf3488a953a4ba0e68c14fc76c0fd31ebe91f`  
		Last Modified: Tue, 13 Sep 2022 04:58:39 GMT  
		Size: 53.4 MB (53447031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
