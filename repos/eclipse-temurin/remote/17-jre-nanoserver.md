## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:036865658a7402bb762f7f1f8bcc7e3cdc47dba905e66215b1353ee31aca799e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.825; amd64
	-	windows version 10.0.17763.3165; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.825; amd64

```console
$ docker pull eclipse-temurin@sha256:ab9904aae9cb20c11ff4580ae31aa03fd56c5896d76d91259cd26d66e0e73b44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161322782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfcf4b51def0bab61392211c7b3a405d03096026743c534d4149a55ed095cde4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Jul 2022 15:25:50 GMT
COPY dir:c21630f3252a44226ea19120d87b000e49aedb9d546bbac0f6424fd80f37c64d in C:\openjdk-17 
# Wed, 13 Jul 2022 15:26:05 GMT
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
	-	`sha256:61392dc67ac6623ea1cc4c93c5a2c920877a5fa47db01d8616d02499dcc7dcae`  
		Last Modified: Wed, 20 Jul 2022 12:56:37 GMT  
		Size: 43.1 MB (43124924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f0a21842d88f05d365f0068fba26f407ad0de43a2507e37d6bb93b76479e3a`  
		Last Modified: Wed, 20 Jul 2022 12:56:27 GMT  
		Size: 62.0 KB (61966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull eclipse-temurin@sha256:cd52cfcb007cc35c5d397271673ef4f092839d4f590b1059438cf1c8df8c4002
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149395991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73dc5da071f5c02f01360d1cdd97f0ff31eb02e5426c7ba2e096aee2b70bf449`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Jul 2022 15:13:02 GMT
COPY dir:c21630f3252a44226ea19120d87b000e49aedb9d546bbac0f6424fd80f37c64d in C:\openjdk-17 
# Wed, 13 Jul 2022 15:13:16 GMT
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
	-	`sha256:15bd42b38ee2d2928c3ca6a253b4ae356c22e184a63bc0b6a6846f81f6cfe9aa`  
		Last Modified: Wed, 20 Jul 2022 12:50:48 GMT  
		Size: 43.1 MB (43128651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a98d6d3da009ec0ff394076e24f754cd4f61fc96dc21f86c725e47a109792f7`  
		Last Modified: Wed, 20 Jul 2022 12:50:40 GMT  
		Size: 3.0 MB (3037379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
