## `eclipse-temurin:8u372-b07-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:5b6970248d48ca48832c3fd5a13e2684c7cd884c7a3125dc769240a5b3470d28
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:8u372-b07-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:0059e5ffc65870a07fa2e415c3980f641fcf03b6a043b81bedca1ef08657b187
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160133168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e7dcefcf6be5ed20941103b69f6f57281197865ee34af3bf4e546849c268a9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:08:08 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 01:08:09 GMT
ENV JAVA_HOME=C:\openjdk-8
# Sat, 24 Jun 2023 01:08:09 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:08:27 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:08:27 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:09:17 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Sat, 24 Jun 2023 01:09:31 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbea5bda63402b1122bca84fb83a29eabe3ac42f53b676cae0bf123fbf4c675b`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc47ce762e561d099fa4c5531619dccbef79e567c2089317cda988234f3a6c9`  
		Last Modified: Sat, 24 Jun 2023 01:34:22 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17275874895c99a3d4c099148273b43833a8c576f5394e5bf3c5ac795010045d`  
		Last Modified: Sat, 24 Jun 2023 01:34:20 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693a95809e7399c9b14ef7b1b7d1ec5db3a2a82b8e97ead36e28bf8279f6cea2`  
		Last Modified: Sat, 24 Jun 2023 01:34:21 GMT  
		Size: 78.9 KB (78881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c632d9d479e01e4a9bede0d490011d6332da4af69666d6c9fa716b9f7db3b4b`  
		Last Modified: Sat, 24 Jun 2023 01:34:20 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c344d73e57d6e13f953b106f7586167a7bbaa2cdcac25920eff8dddca400d10e`  
		Last Modified: Sat, 24 Jun 2023 01:35:01 GMT  
		Size: 40.0 MB (39959303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add1e85eea2861f0749f040f110099e6be3ddbb53fb4593892dbbe132d2d3f58`  
		Last Modified: Sat, 24 Jun 2023 01:34:56 GMT  
		Size: 60.9 KB (60931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
