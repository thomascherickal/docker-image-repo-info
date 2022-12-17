## `openjdk:21-ea-2-nanoserver-1809`

```console
$ docker pull openjdk@sha256:b3e076eacc441b159b6588f8fa4114a098a428c926802a3993598ab5b14e3ef9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `openjdk:21-ea-2-nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull openjdk@sha256:a115baf23bf41ceae4b5575ce64ba291bbe1e17bd31fbddbd61001a453a45788
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.5 MB (304460590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff007ef95c25230c31538c59fcf917e901183c11bf1beffe628658fa87e5a63`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Tue, 13 Dec 2022 22:53:34 GMT
SHELL [cmd /s /c]
# Wed, 14 Dec 2022 02:56:32 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 14 Dec 2022 02:56:33 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 02:57:29 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Dec 2022 02:57:30 GMT
USER ContainerUser
# Fri, 16 Dec 2022 23:25:24 GMT
ENV JAVA_VERSION=21-ea+2
# Fri, 16 Dec 2022 23:25:42 GMT
COPY dir:636bb8729ec18b0f7fa1c5a9f81601e7d1126e396f840b7039c4cd93a3d25d2e in C:\openjdk-21 
# Fri, 16 Dec 2022 23:26:16 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 16 Dec 2022 23:26:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fe06cbef5ac46e54edd743daf1bc2bfa36b294c7ce9104837061c41a4bde7b`  
		Last Modified: Tue, 13 Dec 2022 23:57:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f403eb4656dcd257924d61f24cde07e6a0bd4ea52ceb2fbb6aabbe94c2b76b67`  
		Last Modified: Wed, 14 Dec 2022 08:47:11 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfa39493326e86ec6b2f2fd8125ad183b1ed64b2c3f2a4461f05d827cc0926a`  
		Last Modified: Wed, 14 Dec 2022 08:47:11 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b7523c236c3ef82ccdd5905f89f123933015a7d581e70a248676aa7e3a76df`  
		Last Modified: Wed, 14 Dec 2022 08:47:11 GMT  
		Size: 66.3 KB (66297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063f4c761ac43a960d04eea23db92193fd5460a992bd8ac71186731abb9de13c`  
		Last Modified: Wed, 14 Dec 2022 08:47:09 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6e6d6a4a99c548a18b9ea4f9fdaf6b4103fe04b45bc5425ab1b3f5d2d6f6e`  
		Last Modified: Sat, 17 Dec 2022 02:20:19 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018b90b3be587c23e5d24f708b4efb24b89d1bc4a402212d56c5e9a5f606b5a4`  
		Last Modified: Sat, 17 Dec 2022 02:20:42 GMT  
		Size: 194.0 MB (193953675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f90e8554b1fbb73d133424f016064b2310da05c7a3239ed2803571e4d60d98`  
		Last Modified: Sat, 17 Dec 2022 02:20:20 GMT  
		Size: 3.8 MB (3762612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d397de4055c2a8be505e0dd53e6335ce1cc09e5f69cf8da5152e337faa6acf3`  
		Last Modified: Sat, 17 Dec 2022 02:20:19 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
