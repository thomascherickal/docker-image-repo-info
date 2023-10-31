## `eclipse-temurin:21-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:658450c1531743b26bbe69f8c0900390bd8673d6aaf906534e53002e6e5e9cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:21-jre-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:4bf021a46604907409bb0e82b5a610baefb9760c5e97aa156fb0c08cf596ea58
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.4 MB (169436904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f24f6723136ff22af05d9171eeccaa15868ca91d89db94e4b36aa684ece6a50f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Mon, 30 Oct 2023 23:45:02 GMT
COPY dir:a5a397b00294543a7015e10bed54514e1c5f8af5ed3eff5933ba2b604ae103c1 in C:\openjdk-21 
# Mon, 30 Oct 2023 23:45:12 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:9a6df694b842413aa3794ccf15ba18ef23783e2ed27e7a7f7289cff14757f6f8`  
		Last Modified: Mon, 30 Oct 2023 23:58:05 GMT  
		Size: 48.7 MB (48687299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9fab0a100593c27f9a5faa835cd09924e1e8b4a45de9123ebdb55668352648`  
		Last Modified: Mon, 30 Oct 2023 23:57:56 GMT  
		Size: 61.1 KB (61077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:21-jre-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:69c2744c933ac7e7e58dd3304d32184a77fc72cd6ce53bc0fcaeac40717257d2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156593413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb55a8910d056960da5bda63c83f128da822a150649c76fca913e002ccb10c0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Mon, 30 Oct 2023 23:41:29 GMT
COPY dir:a5a397b00294543a7015e10bed54514e1c5f8af5ed3eff5933ba2b604ae103c1 in C:\openjdk-21 
# Mon, 30 Oct 2023 23:41:38 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:a306a2982915e85b9ed133cc0cd9d543ecba89f5599df37dfea87b4707e1c10a`  
		Last Modified: Mon, 30 Oct 2023 23:55:35 GMT  
		Size: 48.7 MB (48688540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79114878fbfdbbf17ec023077fd431457216702d57d310d55b9f9b3827c50297`  
		Last Modified: Mon, 30 Oct 2023 23:55:26 GMT  
		Size: 3.4 MB (3364503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
