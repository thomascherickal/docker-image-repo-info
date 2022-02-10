## `openjdk:17-nanoserver`

```console
$ docker pull openjdk@sha256:a13d5e7a4464f16508cb91c68a706b9558ab0ab8a2cf9358ef7857dfdbddd8e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:17-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:4ee45458de84dfd576ad74c4c77715ba45d04d4cefa7ba630d55cb0a942e2866
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.4 MB (289399180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0a49b82e34ddeba8e250dee82955093128ba59deed834e8d3fb5ff79dadac7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 18:56:54 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 09 Feb 2022 18:56:55 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 18:57:04 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 18:57:05 GMT
USER ContainerUser
# Wed, 09 Feb 2022 18:57:06 GMT
ENV JAVA_VERSION=17.0.2
# Wed, 09 Feb 2022 18:57:36 GMT
COPY dir:09e6dae9f6621f372798a539a0041951600f85effa47175a1c021c5940e0e226 in C:\openjdk-17 
# Wed, 09 Feb 2022 18:57:48 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 09 Feb 2022 18:57:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5a7f567e84a5a148036156650a47ef7eec0187f17e880d3b475e51dacd70077b`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914b81c6940b6f7a401041417a14205bcc3655305688de5d10959584b54f83c2`  
		Last Modified: Wed, 09 Feb 2022 19:28:10 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615018a2d6ca66bc3a1946852b5b023cbfcd685cc7f21b6f3a6e45dd38da6c4b`  
		Last Modified: Wed, 09 Feb 2022 19:28:10 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65bf85f08d2ce475ba272a3efbb2e19cf044aef4cc180cb4b9789a24a6af539`  
		Last Modified: Wed, 09 Feb 2022 19:28:10 GMT  
		Size: 72.9 KB (72935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12638c070af4616e888ef7f6ea57e983bcd8896d7a950a05fc06d15becf36f25`  
		Last Modified: Wed, 09 Feb 2022 19:28:07 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5dde595c414591646076e11d699d28bd0f41544d2892197dbb422b2138c058`  
		Last Modified: Wed, 09 Feb 2022 19:28:07 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e42752641b72fe605108a24f3371c69a83cacc8cab40ae1ae6aa0f88c64348`  
		Last Modified: Wed, 09 Feb 2022 19:28:30 GMT  
		Size: 182.6 MB (182601456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ed94d3c865fcc6d4ae0ebb099e9afe661566b0ddca09b1785d8ec23e57d340`  
		Last Modified: Wed, 09 Feb 2022 19:28:09 GMT  
		Size: 3.6 MB (3630748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9623bf8f41e130fb8ee8812481699b00028976a1dc099efd4b05573afe2120`  
		Last Modified: Wed, 09 Feb 2022 19:28:07 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
