## `golang:1-nanoserver`

```console
$ docker pull golang@sha256:cf289e1c16c026fefce8de0d9b78a6187a7b064a66d1e98ec1c70761bd575e28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `golang:1-nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull golang@sha256:3b6007ec21b7a5d08cafc6a554b463948d2f8cc870125d947e13d9f370c5bcf2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.9 MB (230852993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9567354734de3af4d169941ebc7e3154934edab0ff6557288d4fe94e89b76706`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:56:24 GMT
SHELL [cmd /S /C]
# Wed, 15 Feb 2023 23:56:25 GMT
ENV GOPATH=C:\go
# Wed, 15 Feb 2023 23:56:26 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:57:18 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 15 Feb 2023 23:57:18 GMT
USER ContainerUser
# Wed, 08 Mar 2023 00:24:42 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:27:21 GMT
COPY dir:ba7807802ed24328b363fd1db731e4c016063d2f2ee48aec17d5bb33bef460c8 in C:\Program Files\Go 
# Wed, 08 Mar 2023 00:28:14 GMT
RUN go version
# Wed, 08 Mar 2023 00:28:15 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a1068ea860cf7cfcf2570b406077f352946c2ab4e7cc47dafeea0ad296184c`  
		Last Modified: Thu, 16 Feb 2023 00:29:48 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5accf48cd2ca9b22d7853e0fb83e7425912d2ff4f328ea94b968a3d057bf45`  
		Last Modified: Thu, 16 Feb 2023 00:29:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0fce707085b8c6ba4d885bbdf7fcf641a6ba4ed3684e6ba92f9a13c2f97977`  
		Last Modified: Thu, 16 Feb 2023 00:29:48 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b532fd5c97f06791810fb6ca872ebaa5eeef0fe21bb6b84b9a8016b58f607e4`  
		Last Modified: Thu, 16 Feb 2023 00:29:48 GMT  
		Size: 85.3 KB (85345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c3af22cc381cf6bd474dc13ffa7883d77f0c834443d4087de0d2a5da7775ea`  
		Last Modified: Thu, 16 Feb 2023 00:29:46 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10caf4d512f9fa3daa505b654eefaf374208b88e7ce35284d2c7ce4350d2f9ea`  
		Last Modified: Wed, 08 Mar 2023 00:52:46 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac3be96f26fbcedbf2e84ee65392a2cca39d6c0a4d8b27b0cffa6b5d84eb1ad`  
		Last Modified: Wed, 08 Mar 2023 00:53:23 GMT  
		Size: 108.6 MB (108591767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6570ce6abf0d9f3437ec1fb6db6b67ee5bd4d063b9dd142fdfd5ae23019afe9d`  
		Last Modified: Wed, 08 Mar 2023 00:52:46 GMT  
		Size: 49.6 KB (49608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d6a45ef8c3e5b04dc24246a17600b4ff16ae783a7f19adb2019171a4cacd8`  
		Last Modified: Wed, 08 Mar 2023 00:52:46 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:1-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull golang@sha256:5c29816a113afedb9541230499873c28076a26e2d2c8d5b48386bbde19ca00ba
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215410973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20000984bfd209bdfe181599c532c82c53c6fad51b167135ee82715290f655c3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Thu, 16 Feb 2023 00:01:27 GMT
SHELL [cmd /S /C]
# Thu, 16 Feb 2023 00:01:29 GMT
ENV GOPATH=C:\go
# Thu, 16 Feb 2023 00:01:30 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 00:02:18 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 16 Feb 2023 00:02:19 GMT
USER ContainerUser
# Wed, 08 Mar 2023 00:28:27 GMT
ENV GOLANG_VERSION=1.20.2
# Wed, 08 Mar 2023 00:31:09 GMT
COPY dir:ba7807802ed24328b363fd1db731e4c016063d2f2ee48aec17d5bb33bef460c8 in C:\Program Files\Go 
# Wed, 08 Mar 2023 00:31:55 GMT
RUN go version
# Wed, 08 Mar 2023 00:31:56 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e6d0fd50a58d89dbedba25508f81ef068969a7464dbe7797043bb469eede73`  
		Last Modified: Thu, 16 Feb 2023 00:30:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f95cfcd78e67edfecb50d89e183f9bba5a5967c1471019defc5d80f0e17116`  
		Last Modified: Thu, 16 Feb 2023 00:30:46 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6965df8b23355f70f37c895345b677ecd5e377912a4899a11495ec836fb722`  
		Last Modified: Thu, 16 Feb 2023 00:30:46 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8227315463395a55769643669cf7eaa724763ea97dacf5e46e61c87a54905aa1`  
		Last Modified: Thu, 16 Feb 2023 00:30:46 GMT  
		Size: 68.9 KB (68858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bacb7d8750df98cc095d4306959cf1e011491952a8c6ace7e6ec61a90c47c4`  
		Last Modified: Thu, 16 Feb 2023 00:30:44 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cb49f2e75c0049adaf3ae4175af460c4e662722abd968cbe5980969bcfd7c1`  
		Last Modified: Wed, 08 Mar 2023 00:53:37 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d7e786a2e5d1d7ee754ed54c1063e232ad058a60fc827737a3cfcde68c6734`  
		Last Modified: Wed, 08 Mar 2023 00:54:12 GMT  
		Size: 108.6 MB (108591920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c485f787d75de2ef0758f9ab0bc02f25ec73c49e5adef299723f9e5936157d88`  
		Last Modified: Wed, 08 Mar 2023 00:53:37 GMT  
		Size: 68.1 KB (68078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28ebe8fc2bf3178703b6f9988545fa714d18130ffd30af32aa561100d941e46`  
		Last Modified: Wed, 08 Mar 2023 00:53:37 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
