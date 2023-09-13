## `mongo:7-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:a2802a0e1255ae0129807fdbdfa65bf6a462e24019b7eb725f64f5dcd63e955f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `mongo:7-nanoserver-ltsc2022` - windows version 10.0.20348.1970; amd64

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
