## `eclipse-temurin:8-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:20784e1243672313e30832af72abbf66b245fd692033eebca15630bd228f213d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `eclipse-temurin:8-jdk-nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:e31cea3b28bc50a5f26a7ecc2d4adf13996c450c7a395686c0084706ba90b4b6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.7 MB (223686438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c017681afbe3038593d037fecd3ae9a18bb4f8dc3ead719fec9803b1df346e4e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:34:04 GMT
ENV JAVA_VERSION=jdk8u362-b09
# Wed, 15 Feb 2023 23:34:05 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Feb 2023 23:34:06 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:34:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:34:26 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:34:38 GMT
COPY dir:8214f6b15a617bff549fa1e8e973ad9cf58dcd41804c9c4d00b4aebf5303ecc4 in C:\openjdk-8 
# Wed, 15 Feb 2023 23:35:08 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a35c9fffe8173c13d87bf21f7de2163ad9db299c1f8071c714dbce581312486`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b632c77d3738a4b0bd36ae23404bf676ce2b151ee71067572209262a0d00369`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cffb264ffd2903e1afbd610e16e75f6727340bc7954f9b679953a0bbf10ea7`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114660912ba2c4f3763f99ae68083aea983bbb7f7e0ad4a0988ffc5908f671a6`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 85.2 KB (85222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a0038a4b64f24aaf7e4ddd119116fbd8796a8a7a59946faab0d2cc474b2f7a`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809d8173f9da9a1cac9ffd3d3debc7ee6fa276b1f4f8a26a7735e482c268d574`  
		Last Modified: Thu, 16 Feb 2023 07:21:18 GMT  
		Size: 101.4 MB (101414545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2cd6d62e7d39033f17db09595be85ce5a337225214c781654b5768f1dff99b`  
		Last Modified: Thu, 16 Feb 2023 07:21:02 GMT  
		Size: 61.8 KB (61786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jdk-nanoserver` - windows version 10.0.17763.4010; amd64

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
