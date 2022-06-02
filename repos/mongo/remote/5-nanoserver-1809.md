## `mongo:5-nanoserver-1809`

```console
$ docker pull mongo@sha256:a9b1bd814199525089abbde575727149bc3351c6e62d54a52153dfc1e4d76406
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `mongo:5-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull mongo@sha256:d845fc3f4dd74dabb2d938b75da635a6848ac686f6583180933cda5bbdac478f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **409.6 MB (409632657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a3251178d67b7423a5ea7d569678f2d45b175d2d3ae57bbe37adc0063d5ae8`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Tue, 10 May 2022 22:32:24 GMT
SHELL [cmd /S /C]
# Wed, 11 May 2022 16:40:31 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 16:40:44 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 11 May 2022 16:40:45 GMT
USER ContainerUser
# Wed, 11 May 2022 16:40:46 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Thu, 02 Jun 2022 18:33:30 GMT
ENV MONGO_VERSION=5.0.9
# Thu, 02 Jun 2022 18:34:00 GMT
COPY dir:92accade5339a6525830f6d2f9c1964da22055a5f6e4a75b19634e461c7601bd in C:\mongodb 
# Thu, 02 Jun 2022 18:34:21 GMT
RUN mongo --version && mongod --version
# Thu, 02 Jun 2022 18:34:22 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 02 Jun 2022 18:34:23 GMT
EXPOSE 27017
# Thu, 02 Jun 2022 18:34:24 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d7d4dec608f59eb9166ff96f59e4f4fcbda08a55e78d630ba39e558b23b3e475`  
		Last Modified: Tue, 10 May 2022 22:59:35 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987cbdd0546a925a5277fca5911acd2464f2d239476fc117cd8a3011bd985189`  
		Last Modified: Wed, 11 May 2022 17:27:18 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded12f0f392c537c7ff213a868a7db1e71d13284232bf441fb1b18802cc2c58a`  
		Last Modified: Wed, 11 May 2022 17:27:16 GMT  
		Size: 67.6 KB (67566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a2b90ac4cd5ddd91d660cc65ee02c9cb8c76798bcfcf2f2659c9392279c54`  
		Last Modified: Wed, 11 May 2022 17:27:16 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010bcf23b940f6ea8fc6a008db1ca8b75afaf2fbcf10edac831c4ea75c2d9146`  
		Last Modified: Wed, 11 May 2022 17:27:16 GMT  
		Size: 263.5 KB (263496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4458f002a5ff8fc07ff0093cd7891af2d5167c95780c923a0b12784660fbe7e6`  
		Last Modified: Thu, 02 Jun 2022 18:49:48 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2f241d845e2c747c507216bc8c9e1755bf554b9c85b60a3b17641367fcaee9`  
		Last Modified: Thu, 02 Jun 2022 18:55:13 GMT  
		Size: 306.1 MB (306086726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c75cbb0fb56c714332f054163679c10bc653a828b347ae4994a4b362431028`  
		Last Modified: Thu, 02 Jun 2022 18:49:46 GMT  
		Size: 73.0 KB (73022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6204099e29c4bbbcdc99ee5710dfbd2b35339190cf8626fc312a86df16f67d7`  
		Last Modified: Thu, 02 Jun 2022 18:49:46 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d59991db55e186feec87e87b997fd33cea141c7e8889de0562d39f54f4093e2`  
		Last Modified: Thu, 02 Jun 2022 18:49:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6da291d4a17ae482905dd5f8c416ffd2a72477477c58eaba9b445cd4759b334`  
		Last Modified: Thu, 02 Jun 2022 18:49:46 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
