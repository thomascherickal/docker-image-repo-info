## `mongo:nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:02b0128eed45f000dd584bffe445e2395b5414eb39abda097bde647e2a66e420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `mongo:nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull mongo@sha256:5e58a37e1cdc56f9f2a4cff08667d0d99fa790a1cb61509c72eaa591b66175cd
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **634.8 MB (634803301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de229985a9fcab3cb5bef7a8ed5164b9aa86f9b97fd281ce71961a3b4774514e`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:56:24 GMT
SHELL [cmd /S /C]
# Thu, 16 Feb 2023 00:46:34 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 00:47:15 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 16 Feb 2023 00:47:15 GMT
USER ContainerUser
# Thu, 16 Feb 2023 00:47:17 GMT
COPY multi:4abffac378fdd7fd5082d54935b2f9dc2024a93fc9837ae8701ac6e024ef02ee in C:\Windows\System32\ 
# Thu, 16 Feb 2023 00:47:17 GMT
ENV MONGO_VERSION=6.0.4
# Thu, 16 Feb 2023 00:48:17 GMT
COPY dir:68661c9bc66199176f558318104ff5aa0937d5a9cd22b931af66fda7826a6f78 in C:\mongodb 
# Thu, 16 Feb 2023 00:49:03 GMT
RUN mongod --version
# Thu, 16 Feb 2023 00:49:04 GMT
VOLUME [C:\data\db C:\data\configdb]
# Thu, 16 Feb 2023 00:49:05 GMT
EXPOSE 27017
# Thu, 16 Feb 2023 00:49:05 GMT
CMD ["mongod" "--bind_ip_all"]
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
	-	`sha256:db214e24db987418d45852de020b518bd1f2775c39acd283d3dc32a2d43a9cd2`  
		Last Modified: Thu, 16 Feb 2023 01:39:07 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a09543181ef38cc231e4c1aeaa8c3659c87805f41b3aa4de1846f7ecafaa5d`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 83.3 KB (83288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778f9c80c9fc406ad9bd5c358bead14d62b3e09a69819cfd63b1fca3591c648f`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c5820762c82f2d8598cdfeec5c188618393712d380c457660230a1e49c1cda`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 267.1 KB (267067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726394b332b54f08d080ed6d531077a9aa912bc7925c66e6c80e6d2cca118b16`  
		Last Modified: Thu, 16 Feb 2023 01:39:05 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487a5e0a0046226bc59b5cc407c024e8eaf658676c1b0cccb5ca02051cabab2e`  
		Last Modified: Thu, 16 Feb 2023 01:40:22 GMT  
		Size: 512.3 MB (512272743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e94b9b64c41c911d396795d37900874b2bc6e20f37e85718c885b1b5d6ce476`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 53.5 KB (53537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4419b89d5de3688e8bd8adba7cacd26a6a8f4ad212d2294c1983afeb8cee45`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefcd5351c904a37071c1cf60ffcf5c13543205c48772492ddd734d33abfb231`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bb3202fd2aa02d048c45b682f76cb1af285fc79d28c85f1d99e52f3cd429db`  
		Last Modified: Thu, 16 Feb 2023 01:39:03 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
