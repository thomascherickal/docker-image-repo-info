## `mongo:6-nanoserver`

```console
$ docker pull mongo@sha256:a28810335a29f832fce143b7ddea8c411a9a5aef9311971e370cc58f52ec570a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1970; amd64
	-	windows version 10.0.17763.4851; amd64

### `mongo:6-nanoserver` - windows version 10.0.20348.1970; amd64

```console
$ docker pull mongo@sha256:a7ad46463180f92528fc5070530416e6064c5912e69581041eeb49984d9eafc6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **638.3 MB (638302329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9836354df219d92737375041d17e7964eb7f61eb0531d149a6cb48e81dc1eea`
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
# Wed, 13 Sep 2023 04:15:35 GMT
ENV MONGO_VERSION=6.0.9
# Wed, 13 Sep 2023 04:16:11 GMT
COPY dir:a12ac6ea695bc7285b3454c2236744267f0c36ac9ece5b695f0b6536580cab18 in C:\mongodb 
# Wed, 13 Sep 2023 04:16:23 GMT
RUN mongod --version
# Wed, 13 Sep 2023 04:16:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:16:24 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:16:25 GMT
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
	-	`sha256:3b87cf8346c8ed6b628a5e21398560b08905819bcb54d7d0cd03fa284eba6c67`  
		Last Modified: Wed, 13 Sep 2023 04:49:15 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3922051b51b0b72ea0f50c6d3ef0150b8de72ddcfd08e3e4e8d6af22e4824c`  
		Last Modified: Wed, 13 Sep 2023 04:50:29 GMT  
		Size: 517.3 MB (517319270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d00a24c8221a8756b277c51539218e0fd13cb4d5a1bffc5d16d44522b8d699a`  
		Last Modified: Wed, 13 Sep 2023 04:49:13 GMT  
		Size: 61.1 KB (61055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b263da10dd480310bc36cd9a44f6ba8889c373f78071a0c42afe6b19080ce7db`  
		Last Modified: Wed, 13 Sep 2023 04:49:13 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e85a44a2ddac5eb59b767eac25b2d25a0049c6ec424275731408e9a9e04d53`  
		Last Modified: Wed, 13 Sep 2023 04:49:13 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a636615452775f691a356980ab6424f97bfdd3615c5f4660497618ad0f409e32`  
		Last Modified: Wed, 13 Sep 2023 04:49:13 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:6-nanoserver` - windows version 10.0.17763.4851; amd64

```console
$ docker pull mongo@sha256:39eec1ebea3907869b7c4747bae33065b3ecdc1c02aa6b6e30e56d408d4c7ceb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **622.2 MB (622206265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:232a04fa6cade1935d9468889c60b0f9116d8471ef80563f4ecedc089d3d1b0b`
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
# Wed, 13 Sep 2023 04:16:38 GMT
ENV MONGO_VERSION=6.0.9
# Wed, 13 Sep 2023 04:17:14 GMT
COPY dir:a12ac6ea695bc7285b3454c2236744267f0c36ac9ece5b695f0b6536580cab18 in C:\mongodb 
# Wed, 13 Sep 2023 04:17:22 GMT
RUN mongod --version
# Wed, 13 Sep 2023 04:17:23 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:17:24 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:17:25 GMT
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
	-	`sha256:ba695e816d22c80378a651d46c8718d4092a23905f8a348ec2ef786ca9afa863`  
		Last Modified: Wed, 13 Sep 2023 04:50:43 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58704064ce7a562f3ba67981b91b592a913d6e94864137b3e59a72035972a929`  
		Last Modified: Wed, 13 Sep 2023 04:51:56 GMT  
		Size: 517.3 MB (517319481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7c7c1b2f4d1a2e1e52e4a7adbc8990ec0a825c95e188b12caa1fd3f263e3b`  
		Last Modified: Wed, 13 Sep 2023 04:50:41 GMT  
		Size: 49.7 KB (49677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce0bd38932ece175fe1fa8b897f8dfa58607b44dfa918e2ad48396027ccfe2b`  
		Last Modified: Wed, 13 Sep 2023 04:50:41 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e3b971634663e49544e194829bc45b295116333553d0c5e400aa352c052bb7`  
		Last Modified: Wed, 13 Sep 2023 04:50:41 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501dec0b3b1d23e9f58b25619e109a48aee1c8975c0e830e8e466684b64748f9`  
		Last Modified: Wed, 13 Sep 2023 04:50:41 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
