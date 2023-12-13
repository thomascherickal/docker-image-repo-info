## `eclipse-temurin:8u392-b08-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:8f2c9864861171ccfbc7ed567f736753ecdb64398e8cc9eba3ea9826640b36e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:8u392-b08-jre-nanoserver` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:d47b06798930b4ba63caadf98b8abe31050df549e9fe73fb99ad8820a3cc72ed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (161021802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d81ade2bb439eb37cba6f9160665059d17f8a2af3f4d14222d2f0d546cf021`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Dec 2023 00:49:14 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:49:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:49:43 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:50:22 GMT
COPY dir:dbdf2dd9ed9894186d74b75beac1320724c73c6994b00118f04985f0ea2b3067 in C:\openjdk-8 
# Wed, 13 Dec 2023 00:50:34 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420e231f6e0404269e9ff487f0ffc079de3deb8c08e9ff31ccb5fda1d1a44ec`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf164bbdfb6f48a324b0a202412c204a0fe367efe5829ef14105bbd65605b66`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e516ed43c06e2b90a2550de28ed9e594a346fd4668e2807446ad69e0744fcd74`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf7cc4c908cb1abf6fe51888bc260f997343bd25220752f0d3b86076713ae1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002dbdb57bb357c987be5ff6bcbc5e3cd108805d231b7f09809337c5f36e2ba1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 85.5 KB (85519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2219f416115f1fbad27502353948edc25fab0d18bd677b2b058840104dbdc94d`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193dbae1a56d927b5f1940dc1bc91493356eac659fb4abb8f955508b96da3b86`  
		Last Modified: Wed, 13 Dec 2023 06:44:44 GMT  
		Size: 40.1 MB (40111351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69fab786bcddc7d58783d4b2ef29b7431f2a40556c8a3f06eea6ea763c5b5cf`  
		Last Modified: Wed, 13 Dec 2023 06:44:38 GMT  
		Size: 62.1 KB (62106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u392-b08-jre-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:43986b273dacd60b13330e65f8af6c16647fd7e01b31db9f8b4b8a9f6381fd19
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144775255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65ce0303f0ea32596f37139de1f31763b591b020b771e3e6a1e3bd3acca39ef6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:14:37 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:14:38 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Dec 2023 00:14:38 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:14:46 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:14:47 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:19:15 GMT
COPY dir:dbdf2dd9ed9894186d74b75beac1320724c73c6994b00118f04985f0ea2b3067 in C:\openjdk-8 
# Wed, 13 Dec 2023 00:19:26 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bb2669772d53e8f301de1ada41d615e723affe44f15257b083be2409bd5db5`  
		Last Modified: Wed, 13 Dec 2023 06:35:07 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44b4904ea6c8d1f239630ac97b4c689e4a94e4c3f279c346157a468f5af1d0c`  
		Last Modified: Wed, 13 Dec 2023 06:35:07 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e9b3456b3ce55c0f25342c3ad8864049bee32fe4283c352ec02292102493e`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b0b8a38ceced0829a908f23f806d1767f63159b0a4a98036518e380d84fd1a`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 68.3 KB (68327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd4cbb70bf2ba8222fea4798880527b533dfeec77bccce2a922cd91dd128ad9`  
		Last Modified: Wed, 13 Dec 2023 06:35:05 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deca0928f66a0c30b393568343eddc54d55945a9ef24b2187fb6de0acfc09153`  
		Last Modified: Wed, 13 Dec 2023 06:36:06 GMT  
		Size: 40.1 MB (40110956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0300bf24d60d31e0c7e22e5b3c2c187e80c9393d166e4e505c752c8082ba059f`  
		Last Modified: Wed, 13 Dec 2023 06:36:00 GMT  
		Size: 80.1 KB (80144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
