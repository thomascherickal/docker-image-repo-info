## `mongo:7-nanoserver`

```console
$ docker pull mongo@sha256:edab1cdae43b0a9670a6be556cb33ddd282863cf8a9a278219ca3a026dcb00e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `mongo:7-nanoserver` - windows version 10.0.20348.1970; amd64

```console
$ docker pull mongo@sha256:7c207dacd59e952f30a36666f45b3cea6169b494e9962ea9ab50970a7811580f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **732.6 MB (732572029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67042a92f965635dc2b7b780b36c6f84f3878758d4d12007cbd33dc749903835`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 01 Sep 2023 00:20:14 GMT
RUN Apply image 10.0.20348.1970
# Wed, 13 Sep 2023 01:45:13 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 04:00:25 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 04:00:30 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Sep 2023 04:00:31 GMT
USER ContainerUser
# Wed, 13 Sep 2023 04:00:32 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 13 Sep 2023 04:00:32 GMT
ENV MONGO_VERSION=7.0.1
# Wed, 13 Sep 2023 04:01:15 GMT
COPY dir:dd7e8197ac0171161d6946ee93a67cf7f770b5ce539a9dc154869493c9e2623b in C:\mongodb 
# Wed, 13 Sep 2023 04:01:27 GMT
RUN mongod --version
# Wed, 13 Sep 2023 04:01:28 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:01:29 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:01:29 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f8cef0759210af9d01a2fb45d79956a2db738bbd3734b7244b17e14ad945cab`  
		Last Modified: Tue, 12 Sep 2023 18:47:39 GMT  
		Size: 120.6 MB (120567584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c795bb9d48e9fa247e549604525fcb2599507cf1008aa1df12036f428ea236d`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d4f6211677cf82e6ed0d87f108ca902b6953cac7069b26a23966ebb167924`  
		Last Modified: Wed, 13 Sep 2023 04:38:18 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409b27824df1096550781d8d27fdafeb1abf5437c93f4d7bce18fdab09d1a67c`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 79.5 KB (79488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01ed47b78f8c73c7cb1a91613a90350ec6f08cbad9f792825e0a51f4f144fd0`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da139f5b1fbe899c90d6c3ef4302993f201f1ed8f81037e8c9b6dcfec78848ec`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 267.2 KB (267173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475b873edf4ce5ddb142047a891fba0c449793f078390e7ec9cf2385fdd308f3`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a793424ec6fbe725f5162f85102ad81c5366e064b480cedfd14e0808556093a`  
		Last Modified: Wed, 13 Sep 2023 04:39:35 GMT  
		Size: 611.6 MB (611589329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cefa2c84c3b29c9787c3bc3199c0ca0728614ba6415a6f0f1d54a751bc99ae`  
		Last Modified: Wed, 13 Sep 2023 04:38:14 GMT  
		Size: 60.7 KB (60683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b9a1d74b205555a12cd05a3431f710be97e64ce4a29458a4c38a42cbf20ce1`  
		Last Modified: Wed, 13 Sep 2023 04:38:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d5257ddd6ee7e2d0102abfb3aab8f4f50dfae7691c1418148c9c13aced5d6a`  
		Last Modified: Wed, 13 Sep 2023 04:38:14 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1440f8f3057e23f226210adfc9ee99d402efa46a59662c07947d843b4fc1d`  
		Last Modified: Wed, 13 Sep 2023 04:38:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:7-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:479471de8bae09d131f5600be050eadf2a2903a111fb0ca3262b3c3afd2fdebc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **716.5 MB (716476156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad95dc3a8be72055264d7f7958bbc8ed31e4513ab248774cdb35c8e83c1f1105`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 29 Aug 2023 16:42:02 GMT
RUN Apply image 10.0.17763.4851
# Wed, 13 Sep 2023 01:47:57 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 04:01:38 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 04:01:43 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Sep 2023 04:01:44 GMT
USER ContainerUser
# Wed, 13 Sep 2023 04:01:45 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 13 Sep 2023 04:01:46 GMT
ENV MONGO_VERSION=7.0.1
# Wed, 13 Sep 2023 04:02:34 GMT
COPY dir:dd7e8197ac0171161d6946ee93a67cf7f770b5ce539a9dc154869493c9e2623b in C:\mongodb 
# Wed, 13 Sep 2023 04:02:45 GMT
RUN mongod --version
# Wed, 13 Sep 2023 04:02:46 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:02:47 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:02:47 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:17ba6b878467260559b72cb6f7e79c829eae67862a09efe87f6dc324f49fc086`  
		Last Modified: Tue, 12 Sep 2023 18:31:40 GMT  
		Size: 104.5 MB (104492504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bbcbc05a0b3c240fc185ae93c7d844ad01c0d60ef9429ad4d230a78065a9ce`  
		Last Modified: Wed, 13 Sep 2023 02:18:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8461d082f0027d9ed1cd74ee8e9e1dbcb1250ea330332f1459c3a74a59e242`  
		Last Modified: Wed, 13 Sep 2023 04:39:52 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d24e4e27b8237cb6af207bc6c651cf8397fd4f0bd0e14d7fea42327ea04aa6`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 70.2 KB (70185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0a145cf1519e52c048521ae1f199df2b6cba60425d6ed0fda7071a4785269e`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482213ad81ac324a084b76c2ce668699bea68dea46dafa1de09c42aac5b042ed`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 267.1 KB (267051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b09a3b256ed18692d6c1f84dc9358ca9037112214db560beb3855470a5498e9`  
		Last Modified: Wed, 13 Sep 2023 04:39:51 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc8f0412d061f8a9105bc3b4d4d27395657897c52080b5dfcc08987b92354a7`  
		Last Modified: Wed, 13 Sep 2023 04:41:06 GMT  
		Size: 611.6 MB (611589166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3396ea430d8b725a33512953236d5da6c70a71e84103160679f876e2e4c4885f`  
		Last Modified: Wed, 13 Sep 2023 04:39:49 GMT  
		Size: 49.8 KB (49798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d8d87be8809a7b5482f6ab96e53945e3bb1c8fc6b23bc61b1d869df4ccdff`  
		Last Modified: Wed, 13 Sep 2023 04:39:49 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10c07faa51d6720e06c74f7139fbd66a40d2eab3ffe4cc90ef00b4c45ac155a`  
		Last Modified: Wed, 13 Sep 2023 04:39:49 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7daa30936afdc1bd055080ef288891d1716fcb9eaa440b1a2501fd48a18508b`  
		Last Modified: Wed, 13 Sep 2023 04:39:49 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
