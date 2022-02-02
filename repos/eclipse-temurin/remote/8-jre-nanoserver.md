## `eclipse-temurin:8-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:468ef453b89e5efb02bb3c8cbda6f7a07b7d9863502de4e088def562c44c9aa7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.473; amd64
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:2ff97a3fbd02e91c9bdd1a68e4a9af5ad50b179bd92d17ef59b2c0d3e7dc6440
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156597669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c200816b37d2b40215894aa4311bee39200502345b6bbe00febcd8139e72c117`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 16 Jan 2022 04:54:46 GMT
RUN Apply image ltsc2022-amd64
# Wed, 26 Jan 2022 19:40:03 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:50:45 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 01 Feb 2022 22:50:46 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Feb 2022 22:50:47 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:51:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:51:06 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:51:53 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Tue, 01 Feb 2022 22:52:11 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:7691725ee3658d154f940d82fd8c3ff07c0dc589a0c9a93df47ed0ede92a76ab`  
		Size: 117.3 MB (117333150 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f9f8c9f771ab6c67c92a4cbe90414c7b9311902f2b42d89abf566df9ac29c8df`  
		Last Modified: Wed, 26 Jan 2022 20:24:57 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9218efa55144890c1cdbe418eac0251e77fd4d83ff95dd2b428f3c7f9e8b2717`  
		Last Modified: Wed, 02 Feb 2022 00:54:29 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf01084e324927b37163983f0c6a43d63097ca20e25a4e41677b062f63c6ff87`  
		Last Modified: Wed, 02 Feb 2022 00:54:28 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b0fbfde202ff1c3cfdbfa18044b2db61f1b21506cc69a7d32f0ecd68c74540`  
		Last Modified: Wed, 02 Feb 2022 00:54:27 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01de1b2eb34ec42c379b51773b58871d76a360a2e44fd48ac27fc5892215ca1b`  
		Last Modified: Wed, 02 Feb 2022 00:54:26 GMT  
		Size: 85.1 KB (85110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfb8a028a090b616c5570716dfcd4e9e117e900b966c61105a6cb45fb24606e`  
		Last Modified: Wed, 02 Feb 2022 00:54:27 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d358e62e4854385a2f8fc48ace4851dd1504a1396f18cab9aa0e88fae60226c`  
		Last Modified: Wed, 02 Feb 2022 00:56:32 GMT  
		Size: 39.1 MB (39111916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426a11844dc2e330cdcf296039ab30b24b5beacd454606f7007ccef5458b524`  
		Last Modified: Wed, 02 Feb 2022 00:56:25 GMT  
		Size: 61.7 KB (61684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-jre-nanoserver` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:313c04fd194a5c89bc2b9a616b5ae859dbdd22384bb8ebdcaa856be0c90ec0e2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142317989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a870b8411bdec4c0326680fe39dbd9a6f49bbb3b6dbb6f37e9744c636fde111c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:20:19 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 01 Feb 2022 22:20:19 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Feb 2022 22:20:20 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:20:38 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:20:38 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:25:53 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Tue, 01 Feb 2022 22:26:04 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e78c8a17b181b5ee6535c053d3b2c85650f349734b9858cef8526bb76643c9b`  
		Last Modified: Wed, 02 Feb 2022 00:42:33 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710ff6b075e15cfa0c71db2df68e9ba3d9dcaee6f30846fb65cfa9384800f680`  
		Last Modified: Wed, 02 Feb 2022 00:42:33 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71c6d2d842ce5e520afb93ba595f86d312e6716a10b39dda8c91d930745fff`  
		Last Modified: Wed, 02 Feb 2022 00:42:30 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e936d7e60e98bf322a916bcb76ac03d1afcdbd0cd4044bfd51f639763c1fedbe`  
		Last Modified: Wed, 02 Feb 2022 00:42:31 GMT  
		Size: 71.0 KB (71002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abbf95538367cd4deb8ae9bfb78a1316ae4e8e1b74132b309bdf80cd83f3156`  
		Last Modified: Wed, 02 Feb 2022 00:42:31 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae78fc6a5a7b58e5b19bd563f733a04b7150875b6829b87ad80fd5463a22d271`  
		Last Modified: Wed, 02 Feb 2022 00:44:48 GMT  
		Size: 39.1 MB (39112282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49201bb427a665882e7eef39ddd36f145071ed41e613d3faf726ec476c62139`  
		Last Modified: Wed, 02 Feb 2022 00:44:05 GMT  
		Size: 82.4 KB (82416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
