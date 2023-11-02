## `eclipse-temurin:8-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:9df78ae47094bd8477830b14914a7f04f55edc7e64cb729866b0cf728e7f782d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8-jdk-nanoserver-1809` - windows version 10.0.17763.4974; amd64

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
