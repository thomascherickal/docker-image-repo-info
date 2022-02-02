## `eclipse-temurin:8-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:a13ab3c57e2bb26d20ed9d0315deff1f3e58f46cde0ef12b3e73b478e8ebbd56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.473; amd64

### `eclipse-temurin:8-nanoserver-ltsc2022` - windows version 10.0.20348.473; amd64

```console
$ docker pull eclipse-temurin@sha256:c9bdf23c70ee6e24bda1e2cd6c42b13fe25b83ecfff7f86f65f439bd391140c2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.7 MB (217702775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94b8a9b67a6bb48088e6c6cc387540f8dfdbc442097ba5b04d92ed01d800475`
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
# Tue, 01 Feb 2022 22:51:21 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Tue, 01 Feb 2022 22:51:39 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:39ce3b0a406a607f131a804c2318e8c2efea15e0c00463fcc3207a44eacc2103`  
		Last Modified: Wed, 02 Feb 2022 00:56:11 GMT  
		Size: 100.2 MB (100216992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6fef63284b34c7526b9bf8b85de3a818143eb3651d8827d07cc638bdff3215`  
		Last Modified: Wed, 02 Feb 2022 00:54:26 GMT  
		Size: 61.7 KB (61714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
