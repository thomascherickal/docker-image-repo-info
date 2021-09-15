## `eclipse-temurin:16-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:4df1a85ca7a6000db07a064271893a401dd918672fb59e133ec198ced228a92b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `eclipse-temurin:16-jdk-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull eclipse-temurin@sha256:dc4a294d16dde8002aed1aa23d9f874d5b7265568bb0b057712f1bad8da8f624
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305198904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9649931140e75b941b0b15ca4d9c76603d94921775223ce445e408dcdfdbbf36`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 16:36:48 GMT
ENV JAVA_VERSION=jdk-16.0.2+7
# Wed, 15 Sep 2021 16:36:49 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Sep 2021 16:36:50 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 16:36:58 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Sep 2021 16:36:59 GMT
USER ContainerUser
# Wed, 15 Sep 2021 16:37:13 GMT
COPY dir:9a7ef5975d9ba9576c4744dc049616bbcb218f14c3c0bd967851cd46479d6134 in C:\openjdk-16 
# Wed, 15 Sep 2021 16:37:27 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Sep 2021 16:37:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:807d06303c39b2317729754a4c7ad6501e59c16ee464f8f671f9947774f62f72`  
		Last Modified: Wed, 15 Sep 2021 01:10:56 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea14e5698e854748725f78b1676e99f78d778e0d5d8d525533942951b981bb1`  
		Last Modified: Wed, 15 Sep 2021 17:00:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15de317ce490bfe30037a4c6084873d24446b20d228b9058e5f0d9023d34f575`  
		Last Modified: Wed, 15 Sep 2021 17:00:11 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5688dbd245b51605e55e0f21190379a68b3f0c3bafc012c8c5d1a035cb0932`  
		Last Modified: Wed, 15 Sep 2021 17:00:10 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e81e7916df06cccff013e9b8c5fad51742c7c46676fde824e0ec3f4ef9e0971`  
		Last Modified: Wed, 15 Sep 2021 17:00:10 GMT  
		Size: 71.6 KB (71615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b288a97aa0a8af62d0f1dcb10a8e1db3567a6ef16084afdfad8acbbb76e6b0`  
		Last Modified: Wed, 15 Sep 2021 17:00:08 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97436d1bee8816017f40506b91965adef177ba7d7ebe4ce00908ecb0aecf5a8e`  
		Last Modified: Wed, 15 Sep 2021 17:00:26 GMT  
		Size: 198.8 MB (198756974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b286d94fee8b58d7596d32b7091a54f96b93a7f491f87ade895b443583a964`  
		Last Modified: Wed, 15 Sep 2021 17:00:08 GMT  
		Size: 3.7 MB (3660194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03004f4e91a1a2f737270077f6b3c63be45a6ae362027b5848007a85dcec8957`  
		Last Modified: Wed, 15 Sep 2021 17:00:07 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
