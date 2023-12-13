## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a2ff662dd7b2b4eda3d2bbbfe1be8fefc744940ee698ddcdeca52cd0cf9a3efc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:bff67953067ffbc984d77602c90437dbd8c2abed6bdfe99b02bd2c1ee1270966
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164301968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68ba80963f0e07ebe97fe35985fb65a372d052058e4ec5682172131017a3367`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:51:51 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Wed, 13 Dec 2023 00:51:51 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Dec 2023 00:51:52 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:52:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:52:02 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:52:50 GMT
COPY dir:d3f692ac99669197443250e31cbc5c2f5282787fd78589cc9b6c2e91236738f4 in C:\openjdk-17 
# Wed, 13 Dec 2023 00:53:01 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:aa038ec69088a3bbdf7604667f8d479dd0f4f5a0168041e9d805e42d618d493c`  
		Last Modified: Wed, 13 Dec 2023 06:45:47 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee9cdad6a05f3ebd961ba6f316debcbb57e87f8dc5102ee51dfa5029e327831`  
		Last Modified: Wed, 13 Dec 2023 06:45:47 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb62347662c32dbd9a5059bee46400d1afe536c1ed47f79206f5759e84fe9cb`  
		Last Modified: Wed, 13 Dec 2023 06:45:47 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cdb1c73752be1b69a9396ef26b2e184a829632b3b233487e7fb934c324c81a`  
		Last Modified: Wed, 13 Dec 2023 06:45:45 GMT  
		Size: 80.5 KB (80503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20323a48199b46f0117cdc66893cefd6ab328ed9991617295d8004689bb6b86f`  
		Last Modified: Wed, 13 Dec 2023 06:45:45 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15e89ecb5cac8ee707be0554a8b8bd9284c9e47d11d938bac40014f4b75ea2d`  
		Last Modified: Wed, 13 Dec 2023 06:46:22 GMT  
		Size: 43.4 MB (43397617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90147df6124e3d4d31d4dea0daf130a8fb9628ba2f047206d0e0fda443c8ec3d`  
		Last Modified: Wed, 13 Dec 2023 06:46:15 GMT  
		Size: 61.0 KB (61005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:5f81d860b14cd04ec1aa8984e5221214b307efb38fdb75de302f036bcfc74f95
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150957587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739568b7c3f20f88718a854129db39897a68a13d730994253ec215a653d0b090`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:33:45 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Wed, 13 Dec 2023 00:33:45 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 13 Dec 2023 00:33:46 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:33:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:33:55 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:38:33 GMT
COPY dir:d3f692ac99669197443250e31cbc5c2f5282787fd78589cc9b6c2e91236738f4 in C:\openjdk-17 
# Wed, 13 Dec 2023 00:38:44 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:759cb4ed6491f9e54a454d0a71a8f970fc9d89d448f7d1da03704676a4513976`  
		Last Modified: Wed, 13 Dec 2023 06:40:07 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e12f88eba068765157a3c2a27bb0ca228689ff4250045d91de871928ea48ea`  
		Last Modified: Wed, 13 Dec 2023 06:40:06 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428c08e8f690f917aa2abf284c604a53bf62395b8736ae4c634aba98fb676dfa`  
		Last Modified: Wed, 13 Dec 2023 06:40:06 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bd2de65c197e07a96b40407e68be5fe33e9941f893e7904f8b7ddf02f55ef8`  
		Last Modified: Wed, 13 Dec 2023 06:40:04 GMT  
		Size: 68.8 KB (68793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d11b5633cc89d40e3aefdfcc7358f6d8245c3991460c275d523dad5f445bde`  
		Last Modified: Wed, 13 Dec 2023 06:40:04 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3c5d24d06b43f4e0bc18037c08baccfb8d79d62234ac9ff71a63852ff8b86`  
		Last Modified: Wed, 13 Dec 2023 06:41:20 GMT  
		Size: 43.4 MB (43396757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb74c0820c7d89ade0261620ba158bb3988dc3e3cd263acad6580ae09f9ed2`  
		Last Modified: Wed, 13 Dec 2023 06:41:13 GMT  
		Size: 3.0 MB (2976680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
