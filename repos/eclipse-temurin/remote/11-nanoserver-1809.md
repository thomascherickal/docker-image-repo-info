## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:a13fce56da8ffb4a2ee4885fc2fb2d236067b8143ab0623d8a2c633bbb402811
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:c5b2534b2d6b42fc798f206926d04df9080b63a5ae1d08380bb1db960eecc5b3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297732688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab75f067a9740ec47908aeb8e2638b72f75bccc787e32815be144badab0e0673`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:49:23 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Wed, 11 Oct 2023 01:49:24 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 Oct 2023 01:49:24 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:49:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:49:33 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:49:45 GMT
COPY dir:bc17122f89ccac6825b72157f71faf8ee914101def60109a37803e17ec7fe7f6 in C:\openjdk-11 
# Wed, 11 Oct 2023 01:49:58 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 01:49:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c11581d9ee9ea19d58c6cbb415dd809a51b56502169a7a5b301da76d79f63b`  
		Last Modified: Wed, 11 Oct 2023 03:57:05 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79bb5cbcd90cb21698de7c69789381417eaad786834ad21b4d7387014f3e357d`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93cc24fa84d82691bd5a980e6c7b024255c6829f71ce64b7f4f93734979cd03`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df6c958ac9563a101d31a35c6a87b7821c26eec9ddaa8b857cf452d3ee6486`  
		Last Modified: Wed, 11 Oct 2023 07:22:48 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38cb4de6d0643b85e9aa6dcbe1b035b2092f56ee00f2f4fd2cc9a5843c78162`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 65.9 KB (65911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15255fe66122229fa09945bfa11e89e9f85c6c59b0e6885e50fb891fcf98c729`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5f3a51dbb0f14d06408e9244c786c4595b86135328abb5440e5f9db019e814`  
		Last Modified: Wed, 11 Oct 2023 07:23:04 GMT  
		Size: 193.1 MB (193107565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba501b0ec4e39e67138f240b7f0db26c37fb198ce41eeb0c7cd780cede007f7`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 87.7 KB (87744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758144f20f90ef9c8b6436edb159673f0bd85e2312ec2061600b645b0a8025a9`  
		Last Modified: Wed, 11 Oct 2023 07:22:46 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
