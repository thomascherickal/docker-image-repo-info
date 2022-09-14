## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:d5748433a74e70a5c9ebf8709d1a3f9f5a2b416bd6ac19586672f1bff5fa12cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1006; amd64
	-	windows version 10.0.17763.3406; amd64

### `mongo:4-nanoserver` - windows version 10.0.20348.1006; amd64

```console
$ docker pull mongo@sha256:fba87efb1ad97b25180becb16825a8c013df494fa2a14672699f7152b4222f4b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.5 MB (361543357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ff05ca16a528ff58cc49f84a4bd53f3ba8ac0e38ccb219232d7b349c52d04c`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 08 Sep 2022 20:11:22 GMT
RUN Apply image 10.0.20348.1006
# Wed, 14 Sep 2022 12:59:22 GMT
SHELL [cmd /S /C]
# Wed, 14 Sep 2022 18:16:41 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 18:16:54 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Sep 2022 18:16:54 GMT
USER ContainerUser
# Wed, 14 Sep 2022 18:23:48 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Sep 2022 18:35:24 GMT
ENV MONGO_VERSION=4.4.16
# Wed, 14 Sep 2022 18:35:48 GMT
COPY dir:ffbeec6bd323929cd73de85592d4f6ca731152ee6be82baf8e4514fb53642dc6 in C:\mongodb 
# Wed, 14 Sep 2022 18:36:00 GMT
RUN mongo --version && mongod --version
# Wed, 14 Sep 2022 18:36:01 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:36:02 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:36:03 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:09629875cd6ee57fa551626fa2963d8b54718ba9acbf28e7cb5d684a9cb754d7`  
		Size: 118.1 MB (118131331 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:66db2526be0f06c7bd6ba20bdc126ca2d5645acfeb41b5784e4664de37e72b49`  
		Last Modified: Wed, 14 Sep 2022 13:25:26 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f7ad598d1a94ba1f1296571a4da5bf04dde81c7c49e4007c0d7536a959195b`  
		Last Modified: Wed, 14 Sep 2022 19:02:01 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a642c0d7ab9ac57ad706b35c64d641cfc15ba1205447d6102442e8658f3711`  
		Last Modified: Wed, 14 Sep 2022 19:01:59 GMT  
		Size: 99.3 KB (99284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a88827dbafc40e378d95f1d1d7f0924c103f97c9f4ceff294cc2d0eea393aba`  
		Last Modified: Wed, 14 Sep 2022 19:01:59 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8bccb161631572ecd27c567a9f0ef6e1146fbc6093ddb42af4f6b8b55eb929a`  
		Last Modified: Wed, 14 Sep 2022 19:07:35 GMT  
		Size: 263.5 KB (263532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cd590d6d10915a7d28bbbdfc64cca124e15a5ef6f3f5004758bc733aaca6db`  
		Last Modified: Wed, 14 Sep 2022 19:15:19 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2e8ef6faca12ce07e55405f51746b70467f2027663fe8179fb1f5c3b8ce957`  
		Last Modified: Wed, 14 Sep 2022 19:15:59 GMT  
		Size: 243.0 MB (242975966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1558192059b106311dde0056f444059b0024baf8d6d9f2021b33a747c2254777`  
		Last Modified: Wed, 14 Sep 2022 19:15:17 GMT  
		Size: 65.7 KB (65678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4ea726886eeafc1d112acfc7a9db0a7b20004f685274845e695b7f46abdb31`  
		Last Modified: Wed, 14 Sep 2022 19:15:17 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1decfd29bcf31145980b0185264226e8df5804675eb179014e8f13550e0c3910`  
		Last Modified: Wed, 14 Sep 2022 19:15:17 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ceb6580419c36bf0285e76a21ec19ff4e9a9740dcc2a4ecd0719adfc0e8d51`  
		Last Modified: Wed, 14 Sep 2022 19:15:17 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-nanoserver` - windows version 10.0.17763.3406; amd64

```console
$ docker pull mongo@sha256:492205d9c722b8cf5d3daa9cc58bbdb825f90fc2986e119cbcbb38361191cf8e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.7 MB (346731879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66ca9008531331b668262a15b97fee121a0ab4e7da5be877c6e1cb96e098bd7b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 13:03:35 GMT
SHELL [cmd /S /C]
# Wed, 14 Sep 2022 18:18:09 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 18:18:21 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 14 Sep 2022 18:18:22 GMT
USER ContainerUser
# Wed, 14 Sep 2022 18:24:40 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 14 Sep 2022 18:36:09 GMT
ENV MONGO_VERSION=4.4.16
# Wed, 14 Sep 2022 18:36:34 GMT
COPY dir:ffbeec6bd323929cd73de85592d4f6ca731152ee6be82baf8e4514fb53642dc6 in C:\mongodb 
# Wed, 14 Sep 2022 18:36:48 GMT
RUN mongo --version && mongod --version
# Wed, 14 Sep 2022 18:36:49 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 14 Sep 2022 18:36:49 GMT
EXPOSE 27017
# Wed, 14 Sep 2022 18:36:50 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0668477bacdfc2e7df1cd4268b246175ed9b30cf07ccb4bcfcb258d8bee830e`  
		Last Modified: Wed, 14 Sep 2022 13:26:19 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ada06039b3dceb53c91ed6d7bd2d77d0abd90acba1883744d947d1ccee8349`  
		Last Modified: Wed, 14 Sep 2022 19:03:38 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d170c6bf2fd2a53a952e69b17f97ce92dd39dd7294e4b1c6ae6e11adc613210`  
		Last Modified: Wed, 14 Sep 2022 19:03:36 GMT  
		Size: 69.7 KB (69673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16b6830f5e893640af2e263523f5ff88334d46d1a2d69d91cddf1f70f62790`  
		Last Modified: Wed, 14 Sep 2022 19:03:36 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98574a2f866f60f51f05d43d7e4e9d7e62e346b27ff83266400261170b141e2b`  
		Last Modified: Wed, 14 Sep 2022 19:08:41 GMT  
		Size: 263.5 KB (263502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5169bbc0d23b319c08fa275f527adc79650b2f904f10716c9a2b9105314ae7f0`  
		Last Modified: Wed, 14 Sep 2022 19:16:14 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa9518e00e1e86fc17c417ebbed803e3802ab7b42e72e432b9bc94b9ac16859`  
		Last Modified: Wed, 14 Sep 2022 19:16:54 GMT  
		Size: 243.0 MB (242975966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf732d3c3516ca08568867b5a2a5f0fd5e116abfadf3c053902d29475c481e9`  
		Last Modified: Wed, 14 Sep 2022 19:16:12 GMT  
		Size: 81.1 KB (81083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8f2f264d6f51572d4c347b82eae02d9d83457b5ec86869f75dc0d0855cb757`  
		Last Modified: Wed, 14 Sep 2022 19:16:12 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a2538cda1d8280bc3d9cb2b6837aed57aa5127fafc699411b0ff4c56f07c5c`  
		Last Modified: Wed, 14 Sep 2022 19:16:12 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c16e67c9125dd243f456b55ad6ee2244c57ed32a69ab8f2ed2f476ea7ef49b4`  
		Last Modified: Wed, 14 Sep 2022 19:16:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
