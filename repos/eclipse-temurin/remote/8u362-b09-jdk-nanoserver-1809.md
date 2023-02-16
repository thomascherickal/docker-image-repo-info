## `eclipse-temurin:8u362-b09-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:a8722f862a874d0cdc43c4a47a3f19340a2db10936423437ff367d94fdf440d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:8u362-b09-jdk-nanoserver-1809` - windows version 10.0.17763.4010; amd64

```console
$ docker pull eclipse-temurin@sha256:eb92cd11075b2e5e2cc8448ad9265f4d35d9ec198598a2bb6e9b50eab201122d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.2 MB (208241910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc7fa181655801126baca7faf73edbc4fb822df1d63360f0859f6206802dd142`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 22:46:18 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 15 Feb 2023 22:46:19 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Feb 2023 22:46:19 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 22:47:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 22:47:02 GMT
USER ContainerUser
# Wed, 15 Feb 2023 22:47:15 GMT
COPY dir:8214f6b15a617bff549fa1e8e973ad9cf58dcd41804c9c4d00b4aebf5303ecc4 in C:\openjdk-8 
# Wed, 15 Feb 2023 22:47:47 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb76af89064e6926039bd1a5f8e449946c8e3082f3910ce3cf7af0ccb6259c51`  
		Last Modified: Thu, 16 Feb 2023 07:09:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d7b570b79ab848f692285d2a1d32da7c157dd88f451f98698549669abb11c`  
		Last Modified: Thu, 16 Feb 2023 07:09:39 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0808ac41bed3c8cb5a19cadc8bb63c157d8219fbc4d45b1fcc4115eb617a857`  
		Last Modified: Thu, 16 Feb 2023 07:09:37 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997804b0925776e2758cf4996de868021d389b1fae1fe1fe8fe66ea15569b297`  
		Last Modified: Thu, 16 Feb 2023 07:09:36 GMT  
		Size: 76.2 KB (76156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d32ea0f37c1bac419f7ee39433174a6fd29787957a3842e64ad4d8979171367`  
		Last Modified: Thu, 16 Feb 2023 07:09:36 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543bac0cbf47192bf1d1fae90e5469f2676445397ab3ddef6a5054780a317e5a`  
		Last Modified: Thu, 16 Feb 2023 07:09:52 GMT  
		Size: 101.4 MB (101396513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc7df124506ec1d5b0c4e33f2e7881d04d94f4ba265f4a22904d29e426202f`  
		Last Modified: Thu, 16 Feb 2023 07:09:36 GMT  
		Size: 88.5 KB (88453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
