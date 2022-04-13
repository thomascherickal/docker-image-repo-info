## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:30d9472e8c6d32ba3c2a6d7688c8d3d92eadbfd354aeb689674f8764554f68ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:ece1afd4205e3b7275581ba43066cda6a73bcef5a63304572bd0f434d86d3bc2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302742152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37adadcb92268932b2f877c49e9d1626727f59db15dcbae419ed77d2845eab7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:50:04 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 13 Apr 2022 15:50:04 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Apr 2022 15:50:05 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:50:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:50:12 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:50:27 GMT
COPY dir:af72ba1102e9cda7f5ea9974b0cafbe96b2f97690adb0743202a1c732a987a84 in C:\openjdk-17 
# Wed, 13 Apr 2022 15:50:36 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:50:37 GMT
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
	-	`sha256:7aa7a50ad90ae5daac04cfc87bc4f09aefcbbc52453d29a8647dfbd93074d69e`  
		Last Modified: Wed, 13 Apr 2022 16:44:34 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31222ac372d5345ac1a8581900faa54051977f55b5e17e0c4d5457fc4efd781`  
		Last Modified: Wed, 13 Apr 2022 16:44:34 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292a6f81fb8a01823bd6e88bdad7d0a18bb1ec594722f019e3f8fe27d2e1875c`  
		Last Modified: Wed, 13 Apr 2022 16:44:33 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baffabd7d8e6a70ec8f053b4c7128b2b4aeb39199ec12a89724b151343c5cccb`  
		Last Modified: Wed, 13 Apr 2022 16:44:31 GMT  
		Size: 78.1 KB (78070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b329b7a38bc74713731f58cfe1544833130a4dbe6207e90c87d11bf6596bb3`  
		Last Modified: Wed, 13 Apr 2022 16:44:31 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b5f52f379b7e55e0d823d33777aa70a106f07c9b66a9b5d10938e3b6dffeb4`  
		Last Modified: Wed, 13 Apr 2022 16:47:43 GMT  
		Size: 185.0 MB (185017666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630cfde394911dd85d7aedf19790be97ae1e12b3bbdaa96ad64e082ef99ed225`  
		Last Modified: Wed, 13 Apr 2022 16:44:31 GMT  
		Size: 60.8 KB (60809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806d98a6bb4fbcd142da89fc4fbb728a449f86acd0ce256d697de7fd8ad4f158`  
		Last Modified: Wed, 13 Apr 2022 16:44:31 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:00b4289bab0ae24fe3d78ff9cc3043a594ee0849e2666b588d1f0ba6e98219b4
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291824866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9660a60c67daaf2ee31b4964c548e0d0ba947bdb4e6fc4500dddc389ec994d5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:37:47 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Wed, 13 Apr 2022 15:37:48 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Apr 2022 15:37:49 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:37:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:37:56 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:38:10 GMT
COPY dir:af72ba1102e9cda7f5ea9974b0cafbe96b2f97690adb0743202a1c732a987a84 in C:\openjdk-17 
# Wed, 13 Apr 2022 15:38:22 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:38:22 GMT
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
	-	`sha256:15c673da2302df4dcb79c5b7dabb77e1f397e971140f7d7938e9901fdf129f88`  
		Last Modified: Wed, 13 Apr 2022 16:27:19 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70d5e20305f53db451834484636ee7a11afd0bf1ac918d07a034ad86fa47289`  
		Last Modified: Wed, 13 Apr 2022 16:27:18 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7c4a0de67fdccc000e65345b45fabc73816689b9c0e10e43abdd3a6d978ee2`  
		Last Modified: Wed, 13 Apr 2022 16:27:18 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b73b77168ca14497b8087af81bcfdc1c12bf6294ff077284c7b295c94da6bd80`  
		Last Modified: Wed, 13 Apr 2022 16:27:16 GMT  
		Size: 73.1 KB (73055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1db9eebee9ed6a67444d1a78877299c5be7671b6f68d388f5de8040b651edd`  
		Last Modified: Wed, 13 Apr 2022 16:27:15 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a788a198133e07519aa60fa445c61ee54f3fef4df87ff3c3c268fbb4004da5`  
		Last Modified: Wed, 13 Apr 2022 16:27:34 GMT  
		Size: 185.0 MB (185023019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e347ecd41531cd0302278f4c984cd39a155b06c1c14a861fc2fdbb90d74bd6`  
		Last Modified: Wed, 13 Apr 2022 16:27:16 GMT  
		Size: 3.6 MB (3625853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9c82ff303ad77c09479d97bf60f804591585c8b55ab99c21f570431d0abd05`  
		Last Modified: Wed, 13 Apr 2022 16:27:15 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
