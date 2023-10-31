## `eclipse-temurin:21-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:028506576653549d8618dc5c6e0bf06dad3d518e09eb758b0bf346d267a1291e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:21-jre-nanoserver-1809` - windows version 10.0.17763.4974; amd64

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
