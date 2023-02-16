## `eclipse-temurin:8-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:38ae30c0cf2874458ab14b4829c6106220440643c51617aa36f096f6de5441c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:8-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

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
