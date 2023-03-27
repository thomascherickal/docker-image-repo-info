## `openjdk:21-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:651963a066189ba6b6e8f2d209bc4b8319493e2579c38fbbef092db6dbe0aae2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `openjdk:21-ea-nanoserver-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull openjdk@sha256:f02447d749629338ba72f0bb574de7fd226b5402a09bfefea0143d021e6d8102
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306691381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf541dcf20371acd64e93c6d492778c67fccca6717258f633f9bbccb26ef722c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 11 Mar 2023 10:09:02 GMT
RUN Apply image 10.0.17763.4131
# Thu, 16 Mar 2023 00:45:50 GMT
SHELL [cmd /s /c]
# Thu, 16 Mar 2023 04:21:31 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 16 Mar 2023 04:21:32 GMT
USER ContainerAdministrator
# Thu, 16 Mar 2023 04:21:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 16 Mar 2023 04:21:45 GMT
USER ContainerUser
# Mon, 27 Mar 2023 22:25:59 GMT
ENV JAVA_VERSION=21-ea+15
# Mon, 27 Mar 2023 22:26:16 GMT
COPY dir:3ce22bb8439b8874982f894f58fb3a6a808bfaec9a61c4c019c3af11865ca331 in C:\openjdk-21 
# Mon, 27 Mar 2023 22:26:47 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 27 Mar 2023 22:26:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:95eb2f0f3287f5ec687287cc244924aafc74c7ada3121d43f54223487f3f2d8d`  
		Last Modified: Thu, 16 Mar 2023 01:43:14 GMT  
		Size: 106.7 MB (106684240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5837fe68a36caddf38b0aaa99f4ef20ca36d8dfe2825fa6ffbcf0d38b9d59a`  
		Last Modified: Thu, 16 Mar 2023 01:42:43 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450d272e24dcd824ed0a2cfaab457791740701be7e655050f5a344dba0111120`  
		Last Modified: Thu, 16 Mar 2023 04:32:07 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375c9b367947b6469eed8f3b494a27778599dd1e8ab85682d96eee96a8d38097`  
		Last Modified: Thu, 16 Mar 2023 04:32:07 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48b42b9c3192f6ddd8ce43c9c7a2c8b1fb3f906fe4eea3aa9b1e4fc28b4161`  
		Last Modified: Thu, 16 Mar 2023 04:32:08 GMT  
		Size: 72.2 KB (72190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44544dc6ee19ff5b39d3756cbc6d53830c65429f0d1ad05b8422c3c33ac8311`  
		Last Modified: Thu, 16 Mar 2023 04:32:05 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa380d12e450ab115ece020e5bf1ee50a3410e0b40a8174aed931c0bc85fdf9`  
		Last Modified: Mon, 27 Mar 2023 22:30:00 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738580f3be2ac6087d1434eaf33e1ded92298ee17f3198854c5bc23ddf647b90`  
		Last Modified: Mon, 27 Mar 2023 22:30:21 GMT  
		Size: 196.2 MB (196159157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9745daf7757d2e98db06f796e6fc84efef1cf2ff6c334c414d6f8abf7997789`  
		Last Modified: Mon, 27 Mar 2023 22:30:01 GMT  
		Size: 3.8 MB (3768895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e4830f5dad90f8eae442e89f231b48eaaedbe0c21b5c6cbcd902d11e16d1a6`  
		Last Modified: Mon, 27 Mar 2023 22:30:00 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
