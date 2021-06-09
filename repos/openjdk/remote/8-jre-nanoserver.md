## `openjdk:8-jre-nanoserver`

```console
$ docker pull openjdk@sha256:9569bfc7eb9e14eb60caac53b595d33b2fbbc58f73f496de39d61d52a797b88c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1999; amd64

### `openjdk:8-jre-nanoserver` - windows version 10.0.17763.1999; amd64

```console
$ docker pull openjdk@sha256:89726bb1201f5c5b6aeeeee0a4ed2bb590ab3680e818263b115a6c781f78f003
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141015819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:731a38bdc296a1a76b673387bc42444addfec426db550cd73222f5b107df5154`
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
# Wed, 09 Jun 2021 17:20:47 GMT
COPY dir:f730d49fd573406c508c5c18daca9d2bf81afd7c16f0b64747f54fe283bbc615 in C:\openjdk-8 
# Wed, 09 Jun 2021 17:21:04 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:c91337d5ab8383b18eed242bfabc7bc7872e44bc2a557e586515f0baf217c972`  
		Last Modified: Wed, 09 Jun 2021 17:52:19 GMT  
		Size: 38.2 MB (38216823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd78447c11948a79f566da2609d0872e09cfc2959488989d2ed263354512cb1`  
		Last Modified: Wed, 09 Jun 2021 17:51:34 GMT  
		Size: 49.8 KB (49819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
