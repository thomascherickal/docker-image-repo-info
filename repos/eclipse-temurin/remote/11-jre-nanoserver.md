## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:383eef6398fa45889ff88f642a25572311a2459fafff4281892b6a60e04c1e0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.643; amd64

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

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:c6edf0ecb2ba06aae807741b1d4ebadee8eea726fe990a96aa2217573aa26c16
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.0 MB (146016469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d82d3cd667d7045f27442cdfb6c719b6eb17712afda1fc180fc027c513f1a8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:24:50 GMT
ENV JAVA_VERSION=jdk-11.0.14.1+1
# Wed, 13 Apr 2022 15:24:51 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Apr 2022 15:24:51 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:24:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:24:57 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:28:54 GMT
COPY dir:7b430082d92796c7933d8991df8414f6ea317b19767304be325fe29c5d7cc52a in C:\openjdk-11 
# Wed, 13 Apr 2022 15:29:03 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b6ab334c2af7acb91e6cda7ad7606fbbee655eca4963706c53db7e79d778b7`  
		Last Modified: Wed, 13 Apr 2022 16:16:09 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3908978b418e2f4812b09b453a9d2e1d50d50cb59889f23fcdd6c5d9384a2834`  
		Last Modified: Wed, 13 Apr 2022 16:16:09 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0916f40d0dc4b05efd8d50a1a2be795104dd783e99dfb5f992646ba8ef950`  
		Last Modified: Wed, 13 Apr 2022 16:16:09 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44a06aaada9cc5c191ae59370b0fd4fd2f819e702fb6dce5d6bb391f9b5f600`  
		Last Modified: Wed, 13 Apr 2022 16:16:07 GMT  
		Size: 68.4 KB (68370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2489a8731676c96af033a73b9b07eeb6f69b250ab32acefd34e883cfdda52b0f`  
		Last Modified: Wed, 13 Apr 2022 16:16:06 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f21f25eb34fc12d71edc5a0d8deada5742ad4058e0b69407ae91bb16d5884`  
		Last Modified: Wed, 13 Apr 2022 16:21:07 GMT  
		Size: 42.8 MB (42756454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9e14890f10372bb936d40b8162a349b09cf09e03daa4221a1c9f1cc465a6a0`  
		Last Modified: Wed, 13 Apr 2022 16:20:21 GMT  
		Size: 89.8 KB (89841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
