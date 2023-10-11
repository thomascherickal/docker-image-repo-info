## `eclipse-temurin:20-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:08e45018f2fe4227c6a42622894fa9f90d1c1ad05fc3d52ef0d8fcb13fcec4ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:20-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:257705735f6fdd7f950045eeea576aa22664c77cb598931b51c4224696494043
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303786073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec95f7c398715560fc4be5b48220fe3a445eec54720a4d76ebfff4131a6bc160`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:08:43 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Wed, 11 Oct 2023 02:08:44 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 11 Oct 2023 02:08:44 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:08:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:08:54 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:09:07 GMT
COPY dir:4ed074865171ba014f3c2f68f57ad2bb21a4dd6e4cf7ff9654ee6c4c6e5176c0 in C:\openjdk-20 
# Wed, 11 Oct 2023 02:09:18 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 02:09:18 GMT
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
	-	`sha256:8b3995660243563f73dbbc84e0b91410b46a7c1da60b14695abe81d0f1496613`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b88d447d9eced836942706fc967433d907a7092251487a243c8ba882032f97`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c772bbcb4835613302d26f7f49700ec02040b02add8d519052c21a7c3aadab`  
		Last Modified: Wed, 11 Oct 2023 07:28:10 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedee8fa0cf60903a52e89de725fa0b1bc5a681e4ce44b9b9d21572d9dda0017`  
		Last Modified: Wed, 11 Oct 2023 07:28:09 GMT  
		Size: 68.8 KB (68785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd66ef872b8166772391d501b081b022d73c0d160055f785613c9f690c08fa4`  
		Last Modified: Wed, 11 Oct 2023 07:28:08 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d47fcb5112f87a86e47ea0bb947db09dc86f93a51909558e8f79c05b25a6f5`  
		Last Modified: Wed, 11 Oct 2023 07:28:27 GMT  
		Size: 195.5 MB (195463973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab28c3072b96a6c9343b7dbb8025ea85c4a50c2b4096bd29e696d6168351d88`  
		Last Modified: Wed, 11 Oct 2023 07:28:09 GMT  
		Size: 3.8 MB (3781880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3baec7f0690aa3337a43a6e0993ae25cb493766255472982f5f5f9dd26d3507`  
		Last Modified: Wed, 11 Oct 2023 07:28:08 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
