## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:96e49db810845bb82357dac739c6b7a1de5c84a84ea7709a9bfba0304e420625
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:33d3572ba8860cb77a936819374a619661d2ba1245269dd2fe3bf8c0aee6258b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.4 MB (303403609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e24d4da157d93eeada458b503f6327dd2b69b609d30e69a5c46b9732deefbba`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Jul 2022 17:25:17 GMT
RUN Apply image 10.0.20348.825
# Wed, 13 Jul 2022 15:22:06 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:24:51 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 13 Jul 2022 15:24:52 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Jul 2022 15:24:52 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:25:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:25:03 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:25:16 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 13 Jul 2022 15:25:32 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:25:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3719b23d309b17276277110a008a58133c9fc92465d2519f2f32c9961c39887d`  
		Size: 118.0 MB (118046090 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:569505cbc9e1bcad1fbbdd7edca170e5a914864bcad2f53e1fc5d5816ecc8aa5`  
		Last Modified: Wed, 20 Jul 2022 12:54:13 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd304d30701ca0c21239a9af97bd54b9d78f03979db6ff656d7e63f9cd0bd7e2`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69b032ede38561ad345ad0f5cc9ec55cbb7c381193c115d09c752d8718f399b`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785e91de4a68cd7b1fd79bbcfae2f4f57983f5bc22f8b9442034e8ea2fc08e4`  
		Last Modified: Wed, 20 Jul 2022 12:55:55 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6eac017f94e9ccdf56550efc861d11f10c2027f412c844a8a258249c5f541e`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 84.0 KB (83993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fde92d157ca9d16443eea1808f120b1fd10463ad6480c26b750edbd8e640af9`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b694fde26e11baf49a173c5e6e64f4f870fac5037fc3ec8e2d1b03afe0d28b`  
		Last Modified: Wed, 20 Jul 2022 12:56:15 GMT  
		Size: 185.2 MB (185203946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b620d2dedb32ac1b4bb378bdbc1c371e6a07baeac9dae99c61c3ccd95a37fa`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 62.6 KB (62604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9b8d20b337d5816473c1f75be612ac4e2a6513f3cfc0d4a9630a6fb6fb9d9`  
		Last Modified: Wed, 20 Jul 2022 12:55:53 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:49da32ec2d4da5031b17f5c725289eb92163619d0541d1af78ca2053e9a2b3f1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.1 MB (292088965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54f24fcba5f0557d4772856413736215c365d3b60a8ecbaafa114af740de97f7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:08:57 GMT
ENV JAVA_VERSION=jdk-17.0.3+7
# Wed, 13 Jul 2022 15:08:57 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Jul 2022 15:08:58 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:09:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Jul 2022 15:09:09 GMT
USER ContainerUser
# Wed, 13 Jul 2022 15:09:22 GMT
COPY dir:79e149bb8ddfd2a6f3a6975343033743c253d84c3b058ff83fe3162d456d08dd in C:\openjdk-17 
# Wed, 13 Jul 2022 15:09:35 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Jul 2022 15:09:36 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0537b400ca69b94c2c43e3567bb34549a8a564fdb217cff160daa94ae1924ade`  
		Last Modified: Wed, 20 Jul 2022 12:49:24 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9c99b8cb2af9b61bfd7cfad0701801f55ed6c48ca1d76ebdbbb1594ac703a8`  
		Last Modified: Wed, 20 Jul 2022 12:49:24 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661f0e2418e4a1cecf8376e4c9f06b5f6b560c9f8112800534dea2b5a76ac267`  
		Last Modified: Wed, 20 Jul 2022 12:49:24 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8ca4aed23b2a6451646482b4162199eb23717f97f7df21ac7ac3379d4f23f1`  
		Last Modified: Wed, 20 Jul 2022 12:49:22 GMT  
		Size: 69.3 KB (69285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f80c5561eb3e2403be4856706aacffdf88fd3e70bc7734a8820f170ac052e95`  
		Last Modified: Wed, 20 Jul 2022 12:49:22 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd442f9b0937186e4c01d682274379c47eda24fe4278dadaeef86323f2744881`  
		Last Modified: Wed, 20 Jul 2022 12:49:43 GMT  
		Size: 185.2 MB (185206910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778835de193e5085ecaf1eb632643f84b54c06b0a350c44d1ff7f631e6815fb6`  
		Last Modified: Wed, 20 Jul 2022 12:49:23 GMT  
		Size: 3.7 MB (3650930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b4e201dbd437f42a9ec83f4610da27338939ce7f1df7f85e92d7a38414c722`  
		Last Modified: Wed, 20 Jul 2022 12:49:22 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
