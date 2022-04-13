## `eclipse-temurin:17-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:0d34d1dca780cdb1964fb0fb093ecd61df614115642b9cbcd47b35c7628a6ac2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:17-jre-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:ffcb0449b994968eae2e4857a452758eb14b8c48adfb8e0ab499493cc59d2d19
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.3 MB (149287145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d18b9c89f79c498a1e56597af2d125a00c090887dd94880087ee5c58cf058c6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Apr 2022 15:42:20 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Wed, 13 Apr 2022 15:42:30 GMT
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
	-	`sha256:f6e89e47be55512e6b901b7a3676632a82767fb329fa2845e9b12c30755e68cb`  
		Last Modified: Wed, 13 Apr 2022 16:30:24 GMT  
		Size: 43.1 MB (43103065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588d7affed56f98e3ff24c53674aceace7851b07437243460635d4e7eb766248`  
		Last Modified: Wed, 13 Apr 2022 16:29:37 GMT  
		Size: 3.0 MB (3009223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
