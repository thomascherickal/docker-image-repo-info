## `openjdk:8u292-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:cc5f0f034412debfff16ed647da5252b5424fd98bbdb65cc114513c507a5dacb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:8u292-jdk-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:589ae88ad721f0e91a98a7d7fbdf769f5423099c8bf174554b89a11d88255a05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203848135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a80fb88cfc6fc84b35678ea3a67ef145ce5b4b4de97d26646dbf7ec244550e7`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 06 Jun 2021 04:04:04 GMT
RUN Apply image 1809-amd64
# Wed, 09 Jun 2021 16:52:42 GMT
SHELL [cmd /s /c]
# Wed, 09 Jun 2021 17:16:54 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 09 Jun 2021 17:16:56 GMT
USER ContainerAdministrator
# Wed, 09 Jun 2021 17:17:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Jun 2021 17:17:13 GMT
USER ContainerUser
# Wed, 09 Jun 2021 17:17:16 GMT
ENV JAVA_VERSION=8u292
# Wed, 09 Jun 2021 17:17:34 GMT
COPY dir:04533fde1b9ea0cd60bd0fd48d2f644dab91f29f3b0d8a376770cc16b38c53d2 in C:\openjdk-8 
# Wed, 09 Jun 2021 17:17:55 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:e4800203e906d49fbdaf1eeab4de72f28796d5b9a1ea44f8d7461001cfa56614`  
		Size: 102.7 MB (102671454 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:acc28506464ab4d21eaffeb562876f3408463a46d298d12ded7ac0e3dd3c1bd6`  
		Last Modified: Wed, 09 Jun 2021 17:25:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4f0050517ad2ad1dfe686c67ad4edef52695fc36ef84d4e051953f25ac3ff`  
		Last Modified: Wed, 09 Jun 2021 17:49:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bc3df79c65a5d6efe335fc05285533c3fa563058a8e7e3454b08188b6edbcc`  
		Last Modified: Wed, 09 Jun 2021 17:49:49 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185d1d685ea25bbe1d3e73e6bcd2475c9c20bc6f105bfe3f676626415dae3045`  
		Last Modified: Wed, 09 Jun 2021 17:49:46 GMT  
		Size: 71.9 KB (71904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d1c03d3be48127ca3c90ab8611acfa12f40c23e2135c8988f179c911f75fcd`  
		Last Modified: Wed, 09 Jun 2021 17:49:46 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728a6236249cffdec62b9581553b63e9d783ba592cf7565f0e1d8ac9023b46f4`  
		Last Modified: Wed, 09 Jun 2021 17:49:46 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06130955aa4ea4f11fb62f7a8ec359d11fe8544d22f6c5f3bb992930149b67f`  
		Last Modified: Wed, 09 Jun 2021 17:50:03 GMT  
		Size: 101.0 MB (101039649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02eb661ad9a0f29153ee359d74d533b1f7a6ac87577086f545ae34b401f0811`  
		Last Modified: Wed, 09 Jun 2021 17:49:46 GMT  
		Size: 59.3 KB (59309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
