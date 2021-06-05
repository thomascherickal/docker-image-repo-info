## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:1c0843be4b38f3452b46973af86a1479cd682b57091387897fcb824a3740a49f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `mongo:4-nanoserver` - windows version 10.0.17763.1935; amd64

```console
$ docker pull mongo@sha256:098b798fdb43f28fd3580d587c983c83a3170d12eae4f67e94e6107bc72cea98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.5 MB (332467287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9f5efd010d2ba4cd3e29759c6b6454bd3886e2ea80600135f83d2fdbfef2741`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 12:37:28 GMT
SHELL [cmd /S /C]
# Fri, 04 Jun 2021 20:14:32 GMT
USER ContainerAdministrator
# Fri, 04 Jun 2021 20:14:54 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Fri, 04 Jun 2021 20:14:54 GMT
USER ContainerUser
# Fri, 04 Jun 2021 20:14:56 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Fri, 04 Jun 2021 20:16:27 GMT
ENV MONGO_VERSION=4.4.6
# Fri, 04 Jun 2021 20:16:54 GMT
COPY dir:e5731845368f7299600736cac7a9579787821dfbdc9d4f89336700f23196d727 in C:\mongodb 
# Fri, 04 Jun 2021 20:17:16 GMT
RUN mongo --version && mongod --version
# Fri, 04 Jun 2021 20:17:17 GMT
VOLUME [C:\data\db C:\data\configdb]
# Fri, 04 Jun 2021 20:17:18 GMT
EXPOSE 27017
# Fri, 04 Jun 2021 20:17:18 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1476895ad9282252b418d10d28836b6319219a9aa251493772a67af475419a31`  
		Last Modified: Wed, 12 May 2021 12:56:08 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090f158d38919601ba5f861af1e7021daa4a4e4597878e7d9d773c454fb79574`  
		Last Modified: Fri, 04 Jun 2021 20:21:11 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac654470a03bec03c95b136f438af8e1706ebdb353496a3e18e0eda742840ba`  
		Last Modified: Fri, 04 Jun 2021 20:21:08 GMT  
		Size: 69.5 KB (69471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ecf7ac50f004a0d7948ade9e3a4de0d0dc0e9566e41f68bcfd3a5b67f59772`  
		Last Modified: Fri, 04 Jun 2021 20:21:08 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b7e2cae7e5dd4533aa29d94b8a64d192f71fef1d2c3cd856c9504fbe4ee046`  
		Last Modified: Fri, 04 Jun 2021 20:21:08 GMT  
		Size: 274.1 KB (274101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce3f7bdff432cbd95acc47f36eb2d7cbf5dd87af19b33c5b2f244e10fa71203`  
		Last Modified: Fri, 04 Jun 2021 20:22:21 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462f57e917e659fcfbd0ac9c01ab39d605e6c863d33644759e7c0d6f2d79a6ec`  
		Last Modified: Fri, 04 Jun 2021 20:26:53 GMT  
		Size: 230.7 MB (230659034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fcf2f856da7558ca25f8e26531f90df6cd69fd54bcbbad5421f49f28b67b04`  
		Last Modified: Fri, 04 Jun 2021 20:22:19 GMT  
		Size: 81.4 KB (81378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd5e9b513aaecd0bc3d182224eee223b0fd73b1ee97507adfc844b469298b2`  
		Last Modified: Fri, 04 Jun 2021 20:22:19 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930d8ec35ec8caaef730208827a76c89b29054cb234f0269547dc0a9cd121e83`  
		Last Modified: Fri, 04 Jun 2021 20:22:19 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79c2a253f2d613e7e2f3b8ecca7c57131f01a00618012d76f733c904dd0f08`  
		Last Modified: Fri, 04 Jun 2021 20:22:19 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
