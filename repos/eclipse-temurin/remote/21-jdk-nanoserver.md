## `eclipse-temurin:21-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:e5b643e4abf665e756bd4f411adf8bc51fa75b1570f7b0c85577015ba39b1705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:21-jdk-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:b0be1cdb904ef51bb189c11d1abb4b3142fc66a2a43e4f125a179488e0aa00e2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.7 MB (321741633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0be6b3b07b2a66917ebbc5973781bbf75aecc1ceb3d5eb175812a171764d97`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:44:10 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:44:10 GMT
ENV JAVA_HOME=C:\openjdk-21
# Mon, 30 Oct 2023 23:44:11 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:44:19 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:44:19 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:44:32 GMT
COPY dir:fd62014fea6b5cd8b6f3d34ff8f9c5e95aa0ce969b7fd9201e979e77a3abe050 in C:\openjdk-21 
# Mon, 30 Oct 2023 23:44:44 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 30 Oct 2023 23:44:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142fccf33f15e2c503ce4023e2e496d7a99bd036e8b83264772e9dab49c325b3`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a276bb22ff993a1ebaa81caffe09d0b12bb66b9c9190196ebf8157bd4cd7bde0`  
		Last Modified: Mon, 30 Oct 2023 23:57:27 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f8cdc4108d9c1d8efcbb092e409cce46980546a7d70895e984a7651259c0ec`  
		Last Modified: Mon, 30 Oct 2023 23:57:27 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2870bcbcd37f944054271ab4c92ab215cc2cecf38aab50a31fe5ce9b77b6b6f`  
		Last Modified: Mon, 30 Oct 2023 23:57:27 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38122dcf511fbe0cfcf0b32d2ae38bc21047a47d003d795d8734dc9dbf2435e`  
		Last Modified: Mon, 30 Oct 2023 23:57:25 GMT  
		Size: 78.8 KB (78807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80ef838707b6a8b274265302f00ff230c52e3e7b30e72dee59660259f0aa5d3`  
		Last Modified: Mon, 30 Oct 2023 23:57:25 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49aedd1949242de9643f99f1b420b3f00778c84fbf802b443e64e127a7940f2`  
		Last Modified: Mon, 30 Oct 2023 23:57:44 GMT  
		Size: 201.0 MB (200991151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19026bc7c847063e06adb8c9302bdff4cf3735d4af75d8fa4ae374b687bd7a6f`  
		Last Modified: Mon, 30 Oct 2023 23:57:25 GMT  
		Size: 60.9 KB (60922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd1ad1d434e70fc43b5b1304319fe7ce0a98f58947f90733141e6b8290e3d9`  
		Last Modified: Mon, 30 Oct 2023 23:57:25 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-jdk-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:f906e6aaee37a3ea32fd7adcd63a14fb9f6faaaa1eb3fcb5864aa9c74c3415fb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.3 MB (309348179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c516674dec989a60194220064a65fcf2a7eabfe56e94bf1b0d332abd5c1326f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:37:10 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Mon, 30 Oct 2023 23:37:10 GMT
ENV JAVA_HOME=C:\openjdk-21
# Mon, 30 Oct 2023 23:37:11 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:37:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:37:19 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:37:31 GMT
COPY dir:fd62014fea6b5cd8b6f3d34ff8f9c5e95aa0ce969b7fd9201e979e77a3abe050 in C:\openjdk-21 
# Mon, 30 Oct 2023 23:37:42 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 30 Oct 2023 23:37:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbfda931f1b6b55facec4e11e09fd74089222efe5be64032de3b0aa284280ff`  
		Last Modified: Mon, 30 Oct 2023 23:54:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bf6c376383ed405a8518da539993d2cbbe85e717387a5eee211fcf77c62572`  
		Last Modified: Mon, 30 Oct 2023 23:54:12 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adf14580fac55fcd0f85736c99cad2889b252fe404adee2377cde3d6230a0b3`  
		Last Modified: Mon, 30 Oct 2023 23:54:12 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81ff8095f1d5023664ddefb58dd604127b4f46ae13990bf91d814d94ec94014`  
		Last Modified: Mon, 30 Oct 2023 23:54:10 GMT  
		Size: 70.0 KB (70003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1ccb38458adf72087ab820f2b444f5136ccdb2bc2315c03975102bc4690693`  
		Last Modified: Mon, 30 Oct 2023 23:54:10 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbeeac21aba52a76d5c3fc9f95b206a1b880b51caea03578c7ce52c05f0e444`  
		Last Modified: Mon, 30 Oct 2023 23:54:29 GMT  
		Size: 201.0 MB (200994805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c969d8fa7a61d23d10137e5545c8400fb591868c2f3112f9259f9543ff560558`  
		Last Modified: Mon, 30 Oct 2023 23:54:11 GMT  
		Size: 3.8 MB (3811870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf4b84445a3cd8369f53a8bd72799050c684fb1dff34e7b112c7bf3d7e51793`  
		Last Modified: Mon, 30 Oct 2023 23:54:10 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
