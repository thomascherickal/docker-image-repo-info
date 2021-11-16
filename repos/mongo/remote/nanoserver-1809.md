## `mongo:nanoserver-1809`

```console
$ docker pull mongo@sha256:286257195731ad20e740e810acbae91b64c0ad5adbafb427f0fac7f436132b62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `mongo:nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull mongo@sha256:3aa9eb58f0e707b66c1a85327409b2802bd7f05e61de46112a3e092b71df8a5c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.0 MB (397000425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bc935985ca25c06f6e593676ba5688cf631ab8d6cb9519f7ae7c6acaf6d7d90`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 13:41:43 GMT
SHELL [cmd /S /C]
# Wed, 10 Nov 2021 19:14:13 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 19:14:28 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 10 Nov 2021 19:14:29 GMT
USER ContainerUser
# Wed, 10 Nov 2021 19:14:30 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Tue, 16 Nov 2021 02:20:51 GMT
ENV MONGO_VERSION=5.0.4
# Tue, 16 Nov 2021 02:21:20 GMT
COPY dir:4fae3f8bc2971f59596da01771c3bfd50912d56b5c7957a9dc3618b6523b15d9 in C:\mongodb 
# Tue, 16 Nov 2021 02:21:47 GMT
RUN mongo --version && mongod --version
# Tue, 16 Nov 2021 02:21:47 GMT
VOLUME [C:\data\db C:\data\configdb]
# Tue, 16 Nov 2021 02:21:48 GMT
EXPOSE 27017
# Tue, 16 Nov 2021 02:21:49 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9fe7a02124d29cd21b5f6d5ea22a1ba3de09099c347d1d0c0e2d89e650ddee00`  
		Last Modified: Wed, 10 Nov 2021 14:07:31 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a0459f3f99e74f05a8457e55c1f306a65f91eb620f2b335f36b49ce70f8d2f`  
		Last Modified: Wed, 10 Nov 2021 19:40:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a90c3faaf1ec3abe7f2c84c50d3e74483cba21bd14918c5273cd7577764bf12c`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 72.1 KB (72092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b354c743ddd6e6dab3fde4cc72bf3fbf21fd4f2f69d57bdb71b204ddbe92c5`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc81adde81af5d22a9d13bbc929d2143462e050a3c821a78a755b210b322b993`  
		Last Modified: Wed, 10 Nov 2021 19:40:57 GMT  
		Size: 274.1 KB (274065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc775e71db0c4dd1b6fab91749505d5b3c63fdbabbc6668e191f1456df918139`  
		Last Modified: Tue, 16 Nov 2021 02:26:08 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6241f5914e4b91752fde2ba63b5d1e670d9195ef2a673190f6e86129c5129dbb`  
		Last Modified: Tue, 16 Nov 2021 02:26:58 GMT  
		Size: 293.8 MB (293813368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b59e27b5d4da6afc85a5abe8262dd49f905a1a999152bb80602733bdb56897`  
		Last Modified: Tue, 16 Nov 2021 02:26:06 GMT  
		Size: 49.9 KB (49898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7edb391e5a0cc62e7883ef12f4d8a0aa475183207f25cf6fffa42554786125`  
		Last Modified: Tue, 16 Nov 2021 02:26:06 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519a7862058cdfeef0bdb2220cfe4f7af3af74b86ab9884f71d1c5ee8e8e5e23`  
		Last Modified: Tue, 16 Nov 2021 02:26:06 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412cdeba9a87fe0d267bc5832a54b02963d342db553f8ab0d9efed5b73c17908`  
		Last Modified: Tue, 16 Nov 2021 02:26:06 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
