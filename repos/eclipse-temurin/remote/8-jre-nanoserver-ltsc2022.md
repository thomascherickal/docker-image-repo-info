## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:264a70d9f0924e8d914a7caa3d7ef4129e42a5105d6d853c6eb10d9df3e2c6bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.473; amd64

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
