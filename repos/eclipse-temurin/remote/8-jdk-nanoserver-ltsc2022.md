## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:2d8d1417356c810100d7836fc1c799692a91be72d733aabb93580b906002d3e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:c988f371e3f5574f6e57ddb5eec17cd8c3d5dc748606dbdb43c20cdd92129452
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221610455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8531a155f9d1c1b57fc96f0467332872fee5a67503e777cc5186b789201e311`
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
# Sat, 24 Jun 2023 01:08:40 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Sat, 24 Jun 2023 01:08:56 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:349942e54d3f69ba93ee68ad73a182ec0dfa09fa6f35b1a73aab02553775e0ad`  
		Last Modified: Sat, 24 Jun 2023 01:34:33 GMT  
		Size: 101.4 MB (101436329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14dbd04ccdaacdddd33e7aca3632aa0f1e6a3520133aa342faa2b0cfc49aff8`  
		Last Modified: Sat, 24 Jun 2023 01:34:20 GMT  
		Size: 61.2 KB (61192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
