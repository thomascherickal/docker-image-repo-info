## `openjdk:16-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:d3c82d8d1f7f26fbabb370868d067f7e2b5fc790c520c254eae6b9fb82ca5a1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1637; amd64

### `openjdk:16-jdk-nanoserver` - windows version 10.0.17763.1637; amd64

```console
$ docker pull openjdk@sha256:b1dd878e025d75928923fd285b1b1e788e55efe77759258c310b714162e656e0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.1 MB (285112614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0679cee8ce902a2dc69ee90c111b0a0b438e920742f3f7bd135231b39c25f9e4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Dec 2020 08:05:47 GMT
RUN Apply image 1809-amd64
# Wed, 09 Dec 2020 18:58:23 GMT
SHELL [cmd /s /c]
# Wed, 09 Dec 2020 18:58:23 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 09 Dec 2020 18:58:24 GMT
USER ContainerAdministrator
# Wed, 09 Dec 2020 18:58:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 09 Dec 2020 18:58:40 GMT
USER ContainerUser
# Fri, 18 Dec 2020 20:19:17 GMT
ENV JAVA_VERSION=16-ea+29
# Fri, 18 Dec 2020 20:19:47 GMT
COPY dir:c7e464ce801c4cbe9fa15b7ab5106d79f537453b590030a2793120e8e956cdad in C:\openjdk-16 
# Fri, 18 Dec 2020 20:20:12 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 18 Dec 2020 20:20:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:21be49aa856f07be4e0a677b988e43c04bd595a3c858e58b6c364477bbbf7222`  
		Size: 101.3 MB (101264827 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fe9a51a0164bd1c063cbda08c4e22dc4f5d04a8047a3951d7441f37fb93c57f2`  
		Last Modified: Wed, 09 Dec 2020 19:34:04 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8993beeae33a05d68775319a4b9f9df44ac08ccfc62cb15113a36b06ad62d1f`  
		Last Modified: Wed, 09 Dec 2020 19:34:02 GMT  
		Size: 869.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340da9582f81cba4147b5da6d500dacd9f3ffdd520c3211dfb20153cd4ae71fc`  
		Last Modified: Wed, 09 Dec 2020 19:34:02 GMT  
		Size: 861.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f848f35781549a8c193011c95049cd95311b558af39d0f8057a5b460a459488`  
		Last Modified: Wed, 09 Dec 2020 19:34:02 GMT  
		Size: 64.6 KB (64579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636f94045101715dca150f5013879c45929dec9e849eac5b53631727e42bb8a6`  
		Last Modified: Wed, 09 Dec 2020 19:33:59 GMT  
		Size: 873.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec1df89b41f0d3958b6d535f4cc73bf47664d0c5df66e0f25ecae726fb6231d`  
		Last Modified: Fri, 18 Dec 2020 20:26:26 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a936582e164e7aae6e41d39fc8b73a120aa2c84d236c1c9b5d93ee42c556826`  
		Last Modified: Fri, 18 Dec 2020 20:26:43 GMT  
		Size: 180.1 MB (180117273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e783314a904d85d6278e2019e89d00049ac3a2729e4520ccf441f4da94075e`  
		Last Modified: Fri, 18 Dec 2020 20:26:26 GMT  
		Size: 3.7 MB (3660719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202d8daf6273369d6618fc338ba5c02c8b25c6578468a9de08f494f82b3814e7`  
		Last Modified: Fri, 18 Dec 2020 20:26:25 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
