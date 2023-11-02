## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a248bab004633605763975b85cc1aa8b3785f7ec3da958abfc6cd98711efcc4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:4daaf5ae4a2c22df81a5e05cc07bac338cc09c98ad67150a65819fc2691271f5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.4 MB (222446707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694051b69d8dba55d0f62c08008a4368bc61ac370c76ae9b17deaba76bec163a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Thu, 02 Nov 2023 01:29:08 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Thu, 02 Nov 2023 01:29:09 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 02 Nov 2023 01:29:10 GMT
USER ContainerAdministrator
# Thu, 02 Nov 2023 01:29:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 02 Nov 2023 01:29:25 GMT
USER ContainerUser
# Thu, 02 Nov 2023 01:29:37 GMT
COPY dir:d9c44d909d2b41aad5bf6fa4f7c7d36e81063822ae5e7ef30e4851bbe7809503 in C:\openjdk-8 
# Thu, 02 Nov 2023 01:29:50 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:eca651b62b3002c026c9959a9e9fe771e9f5f6d921466075d9eac0843b844f3e`  
		Last Modified: Thu, 02 Nov 2023 01:35:46 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a4dda019903db0644c71140f11e351633ccdb26fbbf27f1612511b147fdaf7`  
		Last Modified: Thu, 02 Nov 2023 01:35:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4a2f18b44a2dbbc87331b598fe2b697473f037035d8b202701a569d8a3e2c0`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262bb2d657e5cfc3b0ccaa6b40f822a41cf9e754f34778ccdb2c919fd1985ec3`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 78.2 KB (78246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943ef65f0686e570e1a8ae625774530a802e34c839d058f642c0d39864485b93`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1a4d2308fcf3cab9ae8adac26ab6cd22e30bb61faeed1cbf18d5bbbd212658`  
		Last Modified: Thu, 02 Nov 2023 01:35:56 GMT  
		Size: 101.7 MB (101696221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece75bc3fe364391d82a78f12e16712b5e2d221323be33ba16decfb229fa1a93`  
		Last Modified: Thu, 02 Nov 2023 01:35:44 GMT  
		Size: 62.1 KB (62090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:537eaf9e42e9debd20a9ebc919e85d84b48c45e48658f9ed7d068b6fa1dd9530
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.3 MB (206315622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b097d76e836b3019b4245e7485e47c351d1f8ab0d8d220d09326ee3e54d931`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Thu, 02 Nov 2023 01:22:14 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Thu, 02 Nov 2023 01:22:15 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 02 Nov 2023 01:22:16 GMT
USER ContainerAdministrator
# Thu, 02 Nov 2023 01:22:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 02 Nov 2023 01:22:33 GMT
USER ContainerUser
# Thu, 02 Nov 2023 01:22:45 GMT
COPY dir:d9c44d909d2b41aad5bf6fa4f7c7d36e81063822ae5e7ef30e4851bbe7809503 in C:\openjdk-8 
# Thu, 02 Nov 2023 01:23:00 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:f4914d263915fbf0afd68429eca1951536d4e61179f53b9c2b70123efa1cfe39`  
		Last Modified: Thu, 02 Nov 2023 01:34:09 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11269fa416b9b88395bc9a7ff26cc3475384657db90b97c044ad82c1c6dcc0e7`  
		Last Modified: Thu, 02 Nov 2023 01:34:09 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8fdd6c5b6d8a6b3b70356cbed1bbefb3015ddbd5f485cef45270cb995a7402`  
		Last Modified: Thu, 02 Nov 2023 01:34:06 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0087d12d059879b6320c02ae46b20c95c70957025eac2e8231cef25144192ce3`  
		Last Modified: Thu, 02 Nov 2023 01:34:07 GMT  
		Size: 69.1 KB (69058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a144be38dc7d1b3df2be13248b793651be71e7b9e87035442b53ab5b4fb679`  
		Last Modified: Thu, 02 Nov 2023 01:34:06 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632602ad7ed3f150561ec8382a2a64affe5996d2c3c8f0c2cff4d62caa544ed2`  
		Last Modified: Thu, 02 Nov 2023 01:34:18 GMT  
		Size: 101.7 MB (101693545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfb80b19e266cd722164ce2476a345845f35d95931609e67c337bc59c31acc9`  
		Last Modified: Thu, 02 Nov 2023 01:34:07 GMT  
		Size: 82.7 KB (82651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
