## `openjdk:8u252-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:268fe1113bc04fa71eb89cf165570374db7488f6db818a5b0ab159a6b52fe967
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:8u252-jre-nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:35ad492caf7018d5a8840c519d39d93265a2c24968f040a5113cd499453719e0
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.7 MB (138654812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b00ef03ee80e0fb24a2e8ae56aabfdb1d2274b9977f990a01991cb642ff5fad3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Tue, 14 Apr 2020 21:42:38 GMT
SHELL [cmd /s /c]
# Tue, 14 Apr 2020 22:09:12 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 14 Apr 2020 22:09:13 GMT
USER ContainerAdministrator
# Tue, 14 Apr 2020 22:09:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 14 Apr 2020 22:09:25 GMT
USER ContainerUser
# Thu, 16 Apr 2020 01:04:35 GMT
ENV JAVA_VERSION=8u252
# Thu, 30 Apr 2020 19:16:35 GMT
COPY dir:efe8678d9be4067f8f1280960ef457f634d7198257f7398711cb683e771f08bd in C:\openjdk-8 
# Thu, 30 Apr 2020 19:16:49 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:895ca47ba9cf1a5b61a0721217cfcc038bbe9a4987c7536321c3ac51ef8e5e0c`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464df3018907c0527ae16790c7ef6af4d221c5a2c0a690ee308cfda190d2ae5e`  
		Last Modified: Tue, 14 Apr 2020 22:28:05 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769a32652de01c0d6233289167835286ca3016229fee54adc998f71929b746bd`  
		Last Modified: Tue, 14 Apr 2020 22:28:05 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf786c0bf7c6b12e21a30f380f2a5fdf5e9c65a9e257beaba2d4787140bc8f2`  
		Last Modified: Tue, 14 Apr 2020 22:28:03 GMT  
		Size: 66.0 KB (66008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441b13590eaa83583b349361ff2920e835efdb191f68c066a858e5485ddbbf3`  
		Last Modified: Tue, 14 Apr 2020 22:28:02 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc28dcec7ca224286dd636d167f55d9f403261f13a05206be188af9727019cb`  
		Last Modified: Thu, 16 Apr 2020 01:15:26 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d83e3219488f26cd0d8f1c90c1f6d32412614612069b8f660cde92b245e3db5e`  
		Last Modified: Thu, 30 Apr 2020 19:19:57 GMT  
		Size: 37.4 MB (37420610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e889665a3208f32f87c5b44836f445391f20d6f8f2dc698ee24a0231c8623`  
		Last Modified: Thu, 30 Apr 2020 19:19:51 GMT  
		Size: 45.5 KB (45532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
