## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:14e2afa9349b5519a32a700edfb48b9996a497210be524d0c1bcf57bf0300308
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:e18cd88c0bdd578b9b0c0bc674b1f922da2a0b9fee95c3633778078e30be4909
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165408956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:565e97805296f9296e7b84757d4baf4a2ad0a31c238f281a48c97e677e8909a4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:35:52 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 23:35:53 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Feb 2023 23:35:54 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:36:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:36:07 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:37:17 GMT
COPY dir:ae8209dfc1a9f024f854c3514bc0c0906475eaa2bd640116685865d2510e5d91 in C:\openjdk-11 
# Wed, 15 Feb 2023 23:37:36 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985430554fb89d662596c204cc828ee8c8780d460dae0d82bdefdbdb41a19aa9`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec87a3c2d56bc7bee3681f3cbf3bcff7b5ea15792be07a26236dfff85cbcb25`  
		Last Modified: Thu, 16 Feb 2023 07:21:49 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71364a1354c17d15bef10666b7737cba0d1756a09889840c1221c1a0a1db64fc`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44388c02ea69efa530973287f79b6b344b60c3ec97e7cd3e3d17b2dbc16609d1`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 85.3 KB (85269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ce2305f078863311e40f625dc48ffdfc5f4e8b4f223f7568e33d4f7be60c70`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd202e35b8ac44bf5e7aca42c8685494d0c2c526fad1b59bf27cd83363afb962`  
		Last Modified: Thu, 16 Feb 2023 07:22:37 GMT  
		Size: 43.1 MB (43137139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e07c09154462d1e4d215695be2320f452b64ef93c01aa176851dddfa5e844a`  
		Last Modified: Thu, 16 Feb 2023 07:22:27 GMT  
		Size: 61.9 KB (61850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:764353fe799a59a555bac5a801d28c43c7961c2a167151ed4d1280b83280b0ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.0 MB (149961063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d247fa098a8db73b367243410eaa182dbdc247d8c3c4f31610c0a9afdc959420`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:00:27 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 23:00:28 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Feb 2023 23:00:29 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:00:42 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:00:43 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:06:39 GMT
COPY dir:ae8209dfc1a9f024f854c3514bc0c0906475eaa2bd640116685865d2510e5d91 in C:\openjdk-11 
# Wed, 15 Feb 2023 23:06:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacd283645088b748f2236c3603cb5b4ca410d489109d7387d2418bceb646a55`  
		Last Modified: Thu, 16 Feb 2023 07:12:39 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef6a2a475b6478f866f64610af04abc980de3ce18fab63fd0a60090584da045`  
		Last Modified: Thu, 16 Feb 2023 07:12:40 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f57adb7c019cf106d5ba65ea8d4d187376ac500274b00a34d353d93b08aecf1`  
		Last Modified: Thu, 16 Feb 2023 07:12:39 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514262b1ee7b992f1767c1bff598e30a20984736a824b8d5844812f2f5403b40`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 69.3 KB (69264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e07a29aba56ecf28c6116fc1547bb56c795f39be19e69650b61b8b680d87e6`  
		Last Modified: Thu, 16 Feb 2023 07:12:37 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ccc83cb07a8317034548bde6acb0d3e68859ebfeb96327217edc0b277a466c`  
		Last Modified: Thu, 16 Feb 2023 07:14:08 GMT  
		Size: 43.1 MB (43130112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119225f1a9777df707e083408a7c9d12ad8d8924f36f68a50b4387bbde07000f`  
		Last Modified: Thu, 16 Feb 2023 07:13:59 GMT  
		Size: 80.9 KB (80909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
