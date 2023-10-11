## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:24532d1430d57f6f7845830eb0cffdd6e15afc3fdb092cbcf2111f4e2a5b1960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:e76aa91db2dbe9d85075a1f23e3f4b79a604471b0b82274513c35d9e7375a310
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160739833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a7f4dba44195b5742d8554526523a9059897f9fa3b802e2fd15b10b99a721ed`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 02:14:41 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:14:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:14:55 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:15:28 GMT
COPY dir:f24575d0fd9e2979f5a8010c202ec6d963a3eb3cd788517e3ab1d758c8e6ad81 in C:\openjdk-8 
# Wed, 11 Oct 2023 02:15:40 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:9e573e8d27715408942370bbe3e31eb4ae2c5feadca2cccb3f642115eb3782d0`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a95305dbe93fdf5eb7909af77dfe59c82075bfa61c017c8df26328dfd9e91f`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfa1af4fca27ac3e9a84f67da56ec595a2803fbb10b8a798ff27458de06a3f8`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe98fb9ff1cdb5c208cddc16e8f295fc8a2f2c4015171e38254517402041f9b7`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 86.2 KB (86233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1c6eb49fa819be7d62d2c434696a6dc3cde2b7a8d4494aceae0bc0c7739b2`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67a267401df6ca6ce1b2a12a5ae3792028abce2a246a07f2590ed80d0025cda`  
		Last Modified: Wed, 11 Oct 2023 07:30:02 GMT  
		Size: 40.0 MB (39981269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8201ff253dc64f4908c06b287b40cb6e82b1a8e160fb56ce643ac1fd39302c`  
		Last Modified: Wed, 11 Oct 2023 07:29:56 GMT  
		Size: 62.2 KB (62226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:fa960c1b12ac5c16101b32036b96aacec6f3332ac30a901cabf3052df0df9f78
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144601824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623817b3d707927f557eaae8e0b3261f56008bcb22389544b2c0893d29c255fb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:39:37 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 01:39:38 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 01:39:39 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:39:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:39:50 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:44:25 GMT
COPY dir:f24575d0fd9e2979f5a8010c202ec6d963a3eb3cd788517e3ab1d758c8e6ad81 in C:\openjdk-8 
# Wed, 11 Oct 2023 01:44:34 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:2bfa6f4a1c2a7c533d18ec0dca92bed309d0669d2afab455d6d5212351b975d7`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170446211d70073742ac91df84068c411612746e25962e9ff96b3e9282f20ca6`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03792e6d164d8cd335567497987aebb8b5b2425e1cddb7bdb44d32a94149ce4c`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa70d1de1a8dca6152d4582a2933b41dd7345f53273a4973ce1d623209c972e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 68.5 KB (68544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d097244be50912160bdc8158894bd41a8b5cc337313348edc3b35420ac656e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3b01699b8f8d8f7eaabafc7d8ebcdaba97c18b4636ab14265da7c28bb28bc`  
		Last Modified: Wed, 11 Oct 2023 07:21:19 GMT  
		Size: 40.0 MB (39981049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9621ed523987576f1d1ef86194b73ba35bdf8a46fcc692a9d484609476f19653`  
		Last Modified: Wed, 11 Oct 2023 07:21:14 GMT  
		Size: 81.9 KB (81857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
