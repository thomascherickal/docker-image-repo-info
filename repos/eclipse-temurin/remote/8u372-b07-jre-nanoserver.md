## `eclipse-temurin:8u372-b07-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:3cb8137b6de2d01e8729642331186cfd320e6a2b71a1c083d2db1caf15b2d0e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:8u372-b07-jre-nanoserver` - windows version 10.0.20348.1787; amd64

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

### `eclipse-temurin:8u372-b07-jre-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:cac14073bd5a70333043c35a1b5f422d35f60db96a14f33d0d4f64c08bbab204
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144512856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f683177ea21a171143e1446d78cc82169ebefe34be4a80ec7e45f0f23d6dace`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 00:41:51 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Sat, 24 Jun 2023 00:41:52 GMT
ENV JAVA_HOME=C:\openjdk-8
# Sat, 24 Jun 2023 00:41:53 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 00:42:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 00:42:05 GMT
USER ContainerUser
# Sat, 24 Jun 2023 00:45:16 GMT
COPY dir:8a6c7975745f12f5841a11f3a56ce128ecca26850fc38f023ad9679c09b008c3 in C:\openjdk-8 
# Sat, 24 Jun 2023 00:45:27 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:09087aac643f57e5e24f95fe0a1c8519d0f93dfcf4500263516c0f3874290109`  
		Last Modified: Fri, 23 Jun 2023 02:23:11 GMT  
		Size: 104.4 MB (104400893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09be2e47b3dff420361e93d34eaadedcfd9549c9be5bd77936370792babf874`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b8d173676a3bebe8b880a2e576e384ab320c958eaa8545385db0739f0cedb2`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fce8525b41ee8db302be09889fee5ba69376f2c6519486b55c8cb1256038610`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582c8ef87488af5189acceabd7a9e4f612a5facbf7909a977059bc8f4cbdd1d7`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b71b624ae67158c8af0256f60f5a37249035a4067bcee97ba9a4758e65f608e`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 70.4 KB (70434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c1cdb7974f0d93a444a7f16f91f3ee0ee5a4766f1781f86e73a91e6ac74aab`  
		Last Modified: Sat, 24 Jun 2023 01:24:41 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b802664ec6d61a0b46ab3287b65c25008db51c2cc57b7ed911cde6536a1ad82`  
		Last Modified: Sat, 24 Jun 2023 01:25:56 GMT  
		Size: 40.0 MB (39952084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4805cbbaf86e87d1560e811c8ee4d4130c323c576a38a1db1f581e4e5901`  
		Last Modified: Sat, 24 Jun 2023 01:25:50 GMT  
		Size: 83.7 KB (83658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
