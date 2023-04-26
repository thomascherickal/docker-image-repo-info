## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7c32c4753fc1f5150b487f1dc4ef7be6c24644c480a7e763f5316a0f72379664
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull eclipse-temurin@sha256:416062b2353fe4153f610504a890731a810347b5b70c7c4ff05f54d630720f91
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.1 MB (296072185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c9354720bccb667ff9c0f17aee38252454acac675e08177016ff330e187e81`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Wed, 26 Apr 2023 19:38:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Wed, 26 Apr 2023 19:38:04 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 26 Apr 2023 19:38:05 GMT
USER ContainerAdministrator
# Wed, 26 Apr 2023 19:38:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Apr 2023 19:38:14 GMT
USER ContainerUser
# Wed, 26 Apr 2023 19:38:29 GMT
COPY dir:124ac1113930ce4049263b0be6b87edbaf53b403e9545bc9faa31b4eed61cbf5 in C:\openjdk-17 
# Wed, 26 Apr 2023 19:38:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Apr 2023 19:38:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a1ec02fa1d12354c3753a642e82d439a151eb4c0fe52d0a95babfcbf24a47a`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86c12c67ae63b7b121d66001fcb205fd8bd4641fdebd02717a7b30049358d61`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85d77dd737462ca8131dfd15ac168bc3279cafd6e812fbe09771dc09b57e216`  
		Last Modified: Wed, 26 Apr 2023 20:05:27 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08ae7a2ea51900ae87c5fcde372760769e9a78a91e3cf0edb6a8c8df38a68d0`  
		Last Modified: Wed, 26 Apr 2023 20:05:25 GMT  
		Size: 74.2 KB (74159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050ed453bb1642ab3df2bb207b1b589342eabede15dc9bf2975f09eb04646ab4`  
		Last Modified: Wed, 26 Apr 2023 20:05:25 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2bd73d5d790366ed9bd3435f03345be473a36f330b6e4a6d8f2cb842a44716`  
		Last Modified: Wed, 26 Apr 2023 20:05:43 GMT  
		Size: 185.5 MB (185536103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e672e5262fde6a857737a934597721222e09ce624fda80f2f3189829f846f308`  
		Last Modified: Wed, 26 Apr 2023 20:05:26 GMT  
		Size: 3.7 MB (3666608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b97f904bcaf84bfdf709990b27c84a8435c2f126d640ec8f0dc2df41a389fa`  
		Last Modified: Wed, 26 Apr 2023 20:05:25 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
