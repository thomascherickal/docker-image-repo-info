## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:fb210b1b51df43c6fa9de26b8dcd7004ab53d62aacd8a5f39eb894faafb14a58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:23fff3a9c5ca3bf1d3a176304c55d239ed8a2647cda85284524ad7a6346379a9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.6 MB (307564677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3898c10b4c3648ed31e3988c5650bfb2abd9e96b3b2054f2cab640b160df25b6`
-	Default Command: `["jshell"]`
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
# Wed, 13 Dec 2023 00:52:15 GMT
COPY dir:abd8f71dbffdebb78ff7b01992fc9930e8aa0c6f2b1d8e6ad05b2a0c8da5ed1e in C:\openjdk-17 
# Wed, 13 Dec 2023 00:52:30 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Dec 2023 00:52:31 GMT
CMD ["jshell"]
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
	-	`sha256:73b4351b0494271be43d0a77f6b180dbd3708665673d450da3833e89161ca359`  
		Last Modified: Wed, 13 Dec 2023 06:46:03 GMT  
		Size: 186.7 MB (186659175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912b27600808ab71a36b07984d533409601a79fbdacde3812f7d75f560f24977`  
		Last Modified: Wed, 13 Dec 2023 06:45:45 GMT  
		Size: 61.0 KB (60994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd09669067071fef3ee0e4af39e8f096c89e1273e683848464e5caf8bc9cde2`  
		Last Modified: Wed, 13 Dec 2023 06:45:45 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:245baa3f255d842f04137c621e39188c43b414cdd5dbdcabc05e64f90ed5608a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.9 MB (294853316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f4bab0bba96bc87647907f914ca477b5c9b47b1fa73352df3b4112073a089e1`
-	Default Command: `["jshell"]`
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
# Wed, 13 Dec 2023 00:34:09 GMT
COPY dir:abd8f71dbffdebb78ff7b01992fc9930e8aa0c6f2b1d8e6ad05b2a0c8da5ed1e in C:\openjdk-17 
# Wed, 13 Dec 2023 00:34:20 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Dec 2023 00:34:21 GMT
CMD ["jshell"]
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
	-	`sha256:d5e3663e44757fc14654ae378721889a80c0da5e335f82297776e75dcfe03e01`  
		Last Modified: Wed, 13 Dec 2023 06:40:22 GMT  
		Size: 186.7 MB (186660894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e316e7a4d6a66a303e1c3a0cd850b7e96852d97427229ad8b7d967468c23818b`  
		Last Modified: Wed, 13 Dec 2023 06:40:05 GMT  
		Size: 3.6 MB (3607244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f41e12201142cccb6b6fb8148910efef4167bd77fed916866553cd532becc1`  
		Last Modified: Wed, 13 Dec 2023 06:40:04 GMT  
		Size: 1.0 KB (1028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
