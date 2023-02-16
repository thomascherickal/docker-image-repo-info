## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:fe27a2d2e91dbe2b1e4d3a7edc0b3f4cda99214fc697bb45758bc7c58798c66a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.4010; amd64

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
