## `eclipse-temurin:16-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:b71bcca30f3a144f5ab436cd0e7bc2163f6316d3d423640d6414adebecf50f2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:16-jdk-nanoserver` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:dc7c15bd5d47e2e9f184c8ce17e247633f7111c93f54df9fd86b417a57975cb7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305231585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad5d0f5e855b9f637b04f1ed81ef80c00e6d607615261486acdd1e8b5cffa28`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 16:52:06 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 25 Aug 2021 16:52:07 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 25 Aug 2021 16:52:07 GMT
USER ContainerAdministrator
# Mon, 13 Sep 2021 18:35:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 13 Sep 2021 18:35:50 GMT
USER ContainerUser
# Mon, 13 Sep 2021 18:36:05 GMT
COPY dir:9a7ef5975d9ba9576c4744dc049616bbcb218f14c3c0bd967851cd46479d6134 in C:\openjdk-16 
# Mon, 13 Sep 2021 18:36:20 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 13 Sep 2021 18:36:22 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a12776ab30b6d659896e608b9a969cd3ea03000dbb8efb6596e0e44b53e8096`  
		Last Modified: Wed, 25 Aug 2021 23:40:34 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef56ac4938c5e062fbc7f883a338399ba46e89400a5c743f933907208a870f8`  
		Last Modified: Wed, 25 Aug 2021 23:40:33 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab976dbb82d1519ece5c29f737c75f65b07e7c7fc0773f40648d06139914fbdd`  
		Last Modified: Wed, 25 Aug 2021 23:40:33 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4307223002d59bf0ba45146567c8cd74a3b2ec63d05c1ffe6e6e3e127d00b4f`  
		Last Modified: Mon, 13 Sep 2021 18:55:53 GMT  
		Size: 73.1 KB (73089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32d654e382b44da7aee86cdb30fb6ce954b239c02779c5d107f02f5a63261e4`  
		Last Modified: Mon, 13 Sep 2021 18:55:54 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0787e0f91c5391780670b5be712225c2961e7d3d782d72ac92e93824dbda8a`  
		Last Modified: Mon, 13 Sep 2021 18:56:11 GMT  
		Size: 198.8 MB (198759500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a8aaf23e937db25eac2c56f060fd310f8d2b3dca008bfec3b808a503932b80`  
		Last Modified: Mon, 13 Sep 2021 18:55:54 GMT  
		Size: 3.7 MB (3651028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb385eb0591ae70c6882e010cae07338706ebc755fe3126a049e4423deb3844`  
		Last Modified: Mon, 13 Sep 2021 18:55:53 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
