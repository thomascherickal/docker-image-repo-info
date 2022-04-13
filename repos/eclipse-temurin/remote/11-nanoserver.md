## `eclipse-temurin:11-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a6fb51ccd501b95a203cc60f4eae4e61cfd643708cc734ab32efc657c6d0e4d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:11-nanoserver` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:0ecb0d4b500327dce2ca58a07c39658a5633817fb57d402d094ba954827b4960
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.8 MB (309848179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d690029a11e3a46d0303140f4e767aedc591ffa3c13006988ee1651c007ce8`
-	Default Command: `["jshell"]`
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
# Wed, 13 Apr 2022 15:49:21 GMT
COPY dir:9ebff3631ec53abdcb6e4f307c52be82361e65c94c68bdde1fa726e2b087ad3f in C:\openjdk-11 
# Wed, 13 Apr 2022 15:49:32 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:49:33 GMT
CMD ["jshell"]
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
	-	`sha256:32a706f00d4a57d665bf3ee7c36d8080c1149ec7f854604bba7160c85b13afb5`  
		Last Modified: Wed, 13 Apr 2022 16:43:22 GMT  
		Size: 192.1 MB (192086909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6eb38e5bcbdf9a185605e3ec2ba67cc5694abe3fa5d1fe7bcc5301ae0d0ff2`  
		Last Modified: Wed, 13 Apr 2022 16:39:43 GMT  
		Size: 91.4 KB (91379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8b164b2580815f3eecdde912c0a97485cd5e55d818092c7ac5bdd444177596`  
		Last Modified: Wed, 13 Apr 2022 16:39:43 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:083eb8f38eb22260ac5a6a56cc142ce6f9b091cf2b819505ae6b9b5890d13f7a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295348892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80295525478ffd5cb69de8b4f24a598aec5096b7b6a1509fbb1f28581783540c`
-	Default Command: `["jshell"]`
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
# Wed, 13 Apr 2022 15:25:11 GMT
COPY dir:9ebff3631ec53abdcb6e4f307c52be82361e65c94c68bdde1fa726e2b087ad3f in C:\openjdk-11 
# Wed, 13 Apr 2022 15:25:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:25:23 GMT
CMD ["jshell"]
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
	-	`sha256:4a0bc1fac24f715180690c79bc9325d23e4629d2ab253ab08fcde63b143e0d4c`  
		Last Modified: Wed, 13 Apr 2022 16:19:28 GMT  
		Size: 192.1 MB (192087889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911de7d222826c50297fcdb0957e32202ddab225fdcb5bde74cdcd55aa4cc7ac`  
		Last Modified: Wed, 13 Apr 2022 16:16:07 GMT  
		Size: 89.7 KB (89709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:621d74e5ace467a747f2e35a8036ee1299e4ca99f214a548b8b9465fc04d2da8`  
		Last Modified: Wed, 13 Apr 2022 16:16:07 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
