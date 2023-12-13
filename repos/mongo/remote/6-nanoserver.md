## `mongo:6-nanoserver`

```console
$ docker pull mongo@sha256:2823d8bc3ae2627fd9cc3b3af383bc2b7df9c158c585dcf558109bcda155c75b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `mongo:6-nanoserver` - windows version 10.0.20348.2159; amd64

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

### `mongo:6-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull mongo@sha256:639e9631bd67e69587744160a4f6e292d3be9ca3e6a51b7e34925f0c6afcbd7b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.3 MB (622334434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb0adeceeb9665f59cd31ff098ce03c0beb624977556a80c2ccbbe11f042b92`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Tue, 12 Dec 2023 23:48:09 GMT
SHELL [cmd /S /C]
# Wed, 13 Dec 2023 01:03:37 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 01:03:49 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Dec 2023 01:03:50 GMT
USER ContainerUser
# Wed, 13 Dec 2023 01:03:51 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Wed, 13 Dec 2023 01:11:52 GMT
ENV MONGO_VERSION=6.0.12
# Wed, 13 Dec 2023 01:12:28 GMT
COPY dir:8559148497dc768ddd11c21dfa76fba54aa7fe60a1051bc30a5cf71e7f4f107f in C:\mongodb 
# Wed, 13 Dec 2023 01:12:39 GMT
RUN mongod --version
# Wed, 13 Dec 2023 01:12:40 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Dec 2023 01:12:41 GMT
EXPOSE 27017
# Wed, 13 Dec 2023 01:12:42 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9220949774e2034b6ae56093a689807cead41d7e03c112bf212d6fd6ffc3451`  
		Last Modified: Wed, 13 Dec 2023 00:06:17 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077c8f290e0a52b1a1207bbc16c42a49bc83e084bceed3092c33b15e46934249`  
		Last Modified: Wed, 13 Dec 2023 01:35:09 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe19dabfcc726b3c17c7b578b312c3a55079210aa312af4e7442f43135bc464`  
		Last Modified: Wed, 13 Dec 2023 01:35:07 GMT  
		Size: 69.1 KB (69055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f0fee4d518cae1fc80b12a10357bcc04b4d37e8f5ebf9692fb09f7cbf93bc`  
		Last Modified: Wed, 13 Dec 2023 01:35:07 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a1a0ed7783aa00bbb7e437e99a5a1f75ebecdf881921b65610e8360145231b`  
		Last Modified: Wed, 13 Dec 2023 01:35:07 GMT  
		Size: 267.2 KB (267192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac64008626ce3c74e6da16829b54d952514e806b0b64e8c4f5d8611ef5c77275`  
		Last Modified: Wed, 13 Dec 2023 01:41:06 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de929f0f2e2d01bbaa4ed8af28a432334d65f95d56ee2feba94788aed1a3d7d`  
		Last Modified: Wed, 13 Dec 2023 01:42:20 GMT  
		Size: 517.4 MB (517399971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c63531b03fcd4b87bdd7620d6abbb51e65e5485f21030c4516242b3232b5c1`  
		Last Modified: Wed, 13 Dec 2023 01:41:04 GMT  
		Size: 80.0 KB (80050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faadf32eeb7a9a40cffcf0ed77cf1f1abe20921e60faa3e7d549adc9e9c8574`  
		Last Modified: Wed, 13 Dec 2023 01:41:04 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59ed232a7c2cf013269d6a959e1ea404742e2945104835290992e1544d697e0`  
		Last Modified: Wed, 13 Dec 2023 01:41:04 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2deda2d39467ff016f2c55ff33d51ed2270f44fc55571d2505b95ef5e0a54`  
		Last Modified: Wed, 13 Dec 2023 01:41:03 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
