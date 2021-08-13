## `eclipse-temurin:16-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:5925ab663126fdc43c2672c8c13d50a8507e8bd774b665f1af8825cf067a79ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `eclipse-temurin:16-jdk-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull eclipse-temurin@sha256:650a556a417f717160cb218cc9980304c2e001ebef091633a7ac6992fb404696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305246774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:974b640aa6591e25e186605732445d857043a5c14c28cac125738fe0666818dc`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 11 Aug 2021 17:30:38 GMT
SHELL [cmd /s /c]
# Fri, 13 Aug 2021 21:57:22 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Fri, 13 Aug 2021 21:57:26 GMT
ENV JAVA_HOME=C:\openjdk-16
# Fri, 13 Aug 2021 21:57:28 GMT
USER ContainerAdministrator
# Fri, 13 Aug 2021 21:57:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%         && setx /M PATH %JAVA_HOME%\bin;%PATH%         && echo Complete.
# Fri, 13 Aug 2021 21:57:47 GMT
USER ContainerUser
# Fri, 13 Aug 2021 21:58:07 GMT
COPY dir:9a7ef5975d9ba9576c4744dc049616bbcb218f14c3c0bd967851cd46479d6134 in C:\openjdk-16 
# Fri, 13 Aug 2021 21:58:30 GMT
RUN echo Verifying install ...     && echo   javac --version && javac --version     && echo   java --version && java --version     && echo Complete.
# Fri, 13 Aug 2021 21:58:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae0a5a946be2ad0e39a8260e454c0060a31a9f7e5be75d1f9038dc13730abc0a`  
		Last Modified: Wed, 11 Aug 2021 18:21:28 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b7c7babaa30c097db33f50a6aacf2ccbbcb5a8a6807f6a3c7d11f2a8a2b0f1`  
		Last Modified: Fri, 13 Aug 2021 22:14:03 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ef01eee80f3517b5338177be0c4aa892087777adc5f2351fc5f6225080ab7d`  
		Last Modified: Fri, 13 Aug 2021 22:14:02 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962d6ebf04bde25a40a2a0c4785f2902e5ea47a595079af97e0f016fe7e625e6`  
		Last Modified: Fri, 13 Aug 2021 22:14:02 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf74cc08e32ebf247b23a667c1b5bc7975b7888c0331c268045f8286993387d`  
		Last Modified: Fri, 13 Aug 2021 22:14:00 GMT  
		Size: 69.7 KB (69670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47da78ad22e2b8edd4007ad8cc8aebf4fa9618b0e99fb2db950ac63ae7155439`  
		Last Modified: Fri, 13 Aug 2021 22:14:00 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f5dbd3ae51c5ca6b0cf5fb0be3c96f628e74e432df0d7c58d1564079b3be9f`  
		Last Modified: Fri, 13 Aug 2021 22:14:21 GMT  
		Size: 198.7 MB (198737315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abc7d9c37d9658470f69db33825ff8017b14ee0e51b604b8b5e83903db4868`  
		Last Modified: Fri, 13 Aug 2021 22:14:01 GMT  
		Size: 3.7 MB (3691580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d7ce1469d81f5730af3074dbe0bc8d37fe3f97c6f48fa9386ac7f156d57037`  
		Last Modified: Fri, 13 Aug 2021 22:14:00 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
