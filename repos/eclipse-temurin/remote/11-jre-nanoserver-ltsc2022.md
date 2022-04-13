## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:f96210c6b25f0b7b405fc55ab90fca09b54058a96fc693183d15917f7eb3b5f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:88c90e5d1022883806373707d1c736545474b9b1f5590a367802a78952f778ba
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160487600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d31d6042a1214c2977c7b1e4773a02d35a4f11e3e72ecdc0c97cf9677954644`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:48:56 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Wed, 13 Apr 2022 15:48:57 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Apr 2022 15:48:58 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:49:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:49:06 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:49:47 GMT
COPY dir:7b430082d92796c7933d8991df8414f6ea317b19767304be325fe29c5d7cc52a in C:\openjdk-11 
# Wed, 13 Apr 2022 15:49:57 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:924a7c42e559a85c0bc74dbb028ddeee43fe67b0f59c81c60cbda0082e0e3ae5`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabd9158f10a59f67c9db7d2b6b5e2450cd7ee100f67e1d9a2a31db8ee706954`  
		Last Modified: Wed, 13 Apr 2022 16:39:46 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b4e3d3117c59d53d82dcc4a0fcfe17cb8aa102a9099da7068bfca17cb8123c`  
		Last Modified: Wed, 13 Apr 2022 16:39:46 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baba83cc033876f7328bda13ec6f6394c0fc58a97a2c3ec7b0c99710f62c0304`  
		Last Modified: Wed, 13 Apr 2022 16:39:45 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f58f9d49e38288bb3bd006510c03e75b2b71b3fcde62effe29efb9acf4600b8`  
		Last Modified: Wed, 13 Apr 2022 16:39:43 GMT  
		Size: 84.3 KB (84254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c719554360c39634185628d9dd330a85338bc2fc405486ace78f04526f56071`  
		Last Modified: Wed, 13 Apr 2022 16:39:43 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0adbef5e4061505cc0042a19b002d4b42036c6003255ab04742df83be6a5ac`  
		Last Modified: Wed, 13 Apr 2022 16:44:22 GMT  
		Size: 42.8 MB (42757010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198e7a78977107dd87592b7ac5fabf582ad7aefa4c55768b72df9038626bf3fe`  
		Last Modified: Wed, 13 Apr 2022 16:43:37 GMT  
		Size: 61.7 KB (61726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
