## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:d9bc510ed32a57367aea4a26339f90f8cabfa07e9d89b1ba6bc604e20bd1090a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:7307010b86801c3e033cc76b31e77b816ca4248a57846766a651aeff735675ae
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.2 MB (315174229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73ea30aa6aef46896ce57c995cd090c2d4728aaf01537725f9a4204d2f614f77`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:35:52 GMT
ENV JAVA_VERSION=jdk-11.0.18+10
# Wed, 15 Feb 2023 23:35:53 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Feb 2023 23:35:54 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:36:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:36:07 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:36:25 GMT
COPY dir:3631bd3b4ae70db635b51d6f7ad3f3254aa758db5b0d079379d506c898ecba14 in C:\openjdk-11 
# Wed, 15 Feb 2023 23:36:53 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Feb 2023 23:36:54 GMT
CMD ["jshell"]
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
	-	`sha256:985430554fb89d662596c204cc828ee8c8780d460dae0d82bdefdbdb41a19aa9`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.1 KB (1093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec87a3c2d56bc7bee3681f3cbf3bcff7b5ea15792be07a26236dfff85cbcb25`  
		Last Modified: Thu, 16 Feb 2023 07:21:49 GMT  
		Size: 1.1 KB (1060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71364a1354c17d15bef10666b7737cba0d1756a09889840c1221c1a0a1db64fc`  
		Last Modified: Thu, 16 Feb 2023 07:21:50 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44388c02ea69efa530973287f79b6b344b60c3ec97e7cd3e3d17b2dbc16609d1`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 85.3 KB (85269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ce2305f078863311e40f625dc48ffdfc5f4e8b4f223f7568e33d4f7be60c70`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6172fdac63e2ebf7730d5fb7f2350051ef80ec3d11984010d7b1cc45d13183e4`  
		Last Modified: Thu, 16 Feb 2023 07:22:15 GMT  
		Size: 192.9 MB (192887804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3671c5a7010e7355218f94a964ca13c74c6e480d5ccbfb433a5c917ac318221`  
		Last Modified: Thu, 16 Feb 2023 07:21:48 GMT  
		Size: 75.4 KB (75428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b638e8afa218700d105ea297c7f4693ec8c211bbb9f4884bc2374c8fa0315f1`  
		Last Modified: Thu, 16 Feb 2023 07:21:47 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
