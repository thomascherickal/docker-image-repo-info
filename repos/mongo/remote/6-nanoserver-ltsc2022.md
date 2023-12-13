## `mongo:6-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:cd4f91821cd9479188dceebcb0366cef0082a13378664d5b38a7951fed847bfe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `mongo:6-nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull mongo@sha256:7b94c5d2e181638e8236cb244d378897887899bb8a2dedfc3e7ba716709ba83b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **638.6 MB (638594403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8da319651fa59b5eabe604bf31e32c410314ffa4b26c75859a3d3ef8d01886dc`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Tue, 12 Dec 2023 23:45:11 GMT
SHELL [cmd /S /C]
# Wed, 13 Dec 2023 01:02:09 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 01:02:19 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Dec 2023 01:02:20 GMT
USER ContainerUser
# Wed, 13 Dec 2023 01:02:21 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 13 Dec 2023 01:10:49 GMT
ENV MONGO_VERSION=6.0.12
# Wed, 13 Dec 2023 01:11:24 GMT
COPY dir:8559148497dc768ddd11c21dfa76fba54aa7fe60a1051bc30a5cf71e7f4f107f in C:\mongodb 
# Wed, 13 Dec 2023 01:11:36 GMT
RUN mongod --version
# Wed, 13 Dec 2023 01:11:37 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:11:37 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:11:38 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc3ebec545c94826aa3c6669246f1a71a4e23595f47bc2ebc52c2f139d553c6`  
		Last Modified: Wed, 13 Dec 2023 00:05:37 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df58d66ca4f72c798fc222ceaeffbd947916097bdb9e0b07c639b347e6d9cf04`  
		Last Modified: Wed, 13 Dec 2023 01:33:36 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97937da5ab0aa596d4656c4b3af437019c80112c4125160968548c6db8116d11`  
		Last Modified: Wed, 13 Dec 2023 01:33:34 GMT  
		Size: 93.4 KB (93379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d0d953404b0d21e39542e8ba09d58a36f21f4aad19d9325ff23949bdfea2aa`  
		Last Modified: Wed, 13 Dec 2023 01:33:34 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f91cb3aacc87731223ba583f06799f0e89e928cde0aec5429d0e45f7ae9e2d4`  
		Last Modified: Wed, 13 Dec 2023 01:33:34 GMT  
		Size: 267.2 KB (267197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2c6d9396fc196e6f662d41e68d495e2517ba64e5adc86ad02f60b3ab7ab8e7`  
		Last Modified: Wed, 13 Dec 2023 01:39:41 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadbbb6c7b2a173c19667e9a73fdbdb749488414a988afce0feb7d2e36175398`  
		Last Modified: Wed, 13 Dec 2023 01:40:52 GMT  
		Size: 517.4 MB (517399900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccecc5981a9b47b02242f38c559b5a127bf5cf2dd26fa2a7bc6ecf7302eb802`  
		Last Modified: Wed, 13 Dec 2023 01:39:39 GMT  
		Size: 68.7 KB (68727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c9c2cd2eec263728a2fcfc24659770d02cf9792d1de9c363171acc4047dfbf`  
		Last Modified: Wed, 13 Dec 2023 01:39:39 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e0f1f9dcdda8cac3d08ba6bb3ab42fd138ea31b68ad56b596afe52b95f4efb`  
		Last Modified: Wed, 13 Dec 2023 01:39:38 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f528c86262e92b8d44854400d88720ba1003699cde32751c2269680c458006`  
		Last Modified: Wed, 13 Dec 2023 01:39:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
