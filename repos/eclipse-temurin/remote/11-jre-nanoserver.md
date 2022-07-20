## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:7c8ea28ddc024aeae2d348bd1d01f559bf2d7ac09744b595840e4b6caf33377b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:8bf4bf6b66ae01ed28ddb540a999cad738ba523c4fc6bff6ab8133f5e0b0228c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160981655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111033c4e26b597a0643b27fbb75137814c27c2b209476393bcde6de182f9b04`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:23:21 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 13 Jul 2022 15:23:22 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Jul 2022 15:23:23 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:23:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:23:34 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:24:30 GMT
COPY dir:b81e8d840693600453cb21437c037772b6cbe813879626cf7da1b40ae8a26737 in C:\openjdk-11 
# Wed, 13 Jul 2022 15:24:45 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:569505cbc9e1bcad1fbbdd7edca170e5a914864bcad2f53e1fc5d5816ecc8aa5`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f1d7ed18ddc442fb4f4a640cfebca04ef586c37324c6ac27e1fc63300f3d45`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8277017e15cde483b8b44a6115b95f99675f7005ee4b62a4a81bdf97c1eac7dd`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f99951dad87e30f27404d1dff1852f7351149213eaf5499bc67a89fdfcf21f4`  
		Last Modified: Wed, 20 Jul 2022 12:54:58 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7b5079facd10880a84cf3d272bad70b33a62fc144d3fc961f2f551d6357c7`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 77.7 KB (77660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd41caaf3f7ae470605597ef2dea693acef178db876628d3f379f7a4e9a70711`  
		Last Modified: Wed, 20 Jul 2022 12:54:56 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5e2d0993bc9dea1d2fb09493dbb24e10795ee5479778f579f5fa4cf4510c7e`  
		Last Modified: Wed, 20 Jul 2022 12:55:43 GMT  
		Size: 42.8 MB (42790782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f842c057fbb98a7a5aac4a8ef4302a638839a67d7ec9573027b11cce6930fba`  
		Last Modified: Wed, 20 Jul 2022 12:55:34 GMT  
		Size: 61.4 KB (61414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:6ada453a565e7dbfb4e00db092d0c1366b4224eef55a98e8f60b3205f9079d91
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146102530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c69584a5582ff337312bf4e4a76ecfe34d63203334e2cfe29fd800915afb19e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 14:59:30 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 13 Jul 2022 14:59:31 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Jul 2022 14:59:32 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 14:59:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 14:59:41 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:03:55 GMT
COPY dir:b81e8d840693600453cb21437c037772b6cbe813879626cf7da1b40ae8a26737 in C:\openjdk-11 
# Wed, 13 Jul 2022 15:04:22 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a44b4109423f62e18da9164482c765f03b13a78c5d72b5d8d19fdf076b46c64`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3923d7358dff5064f6087c0c442b1878b2ac256f295e256dad48f49be8675241`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6b4b5ecf5629dc3d0a883a559f734059e0adb86e4078f853a87ae86b008db3`  
		Last Modified: Wed, 20 Jul 2022 12:46:19 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9585a652a462592aefc444c93997c7c3cf5a9b3129fec8879b5515613bf72380`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 71.3 KB (71294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71a31f96ef3a41839d79e6598b654d911e1b0c88598b4d2f29ad83ed0b4139`  
		Last Modified: Wed, 20 Jul 2022 12:46:17 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293900609d55422661754a4324d30c8b3839f696625997f80163c3bd06bcf38a`  
		Last Modified: Wed, 20 Jul 2022 12:47:44 GMT  
		Size: 42.8 MB (42787281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6872245f79d0c974996458f6e6197c9e376dde4b9983e146ce85fffaf8babaf`  
		Last Modified: Wed, 20 Jul 2022 12:47:35 GMT  
		Size: 83.2 KB (83172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
