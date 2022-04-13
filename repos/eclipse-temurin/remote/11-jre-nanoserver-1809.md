## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:0532556809e1ac4e1cefda8cec98b49a1485f3bc6fccd2c75fd1b9c606ab3745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.2803; amd64

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
