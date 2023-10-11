## `eclipse-temurin:20-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:2e99827ec00edac1e6e945f87437bbbd4a38af365b8edf8d552559b7e3750180
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:20-jdk-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:0c4958b1eb0e2ae2a7c0ea9e5f1a16e36a341339d326c013e2885ffcd6247316
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.2 MB (316220984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cd5470d97fd5f4df4740c826c5ce31a4d5a6d1891338d25ce6f90f6d87096bf`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:18:05 GMT
ENV JAVA_VERSION=jdk-20.0.2+9
# Wed, 11 Oct 2023 02:18:06 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 11 Oct 2023 02:18:07 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:18:16 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:18:20 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:18:33 GMT
COPY dir:4ed074865171ba014f3c2f68f57ad2bb21a4dd6e4cf7ff9654ee6c4c6e5176c0 in C:\openjdk-20 
# Wed, 11 Oct 2023 02:18:46 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 Oct 2023 02:18:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fff54800e03713ba81736f43d985319592fc643a1a32b62dbd5c0ec36549de00`  
		Last Modified: Tue, 10 Oct 2023 17:30:43 GMT  
		Size: 120.6 MB (120604344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142fccf33f15e2c503ce4023e2e496d7a99bd036e8b83264772e9dab49c325b3`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66296962efde1d73635a13d15dde63b8790356f4b33e75fc2a018695d6f2bd3`  
		Last Modified: Wed, 11 Oct 2023 07:31:53 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f5d5ce7690da8c76af31f17ce7be0d39d73b853dbeb062c2bc2c79c56158bb`  
		Last Modified: Wed, 11 Oct 2023 07:31:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8a7ee49f1f2375c9d9a234bb777587d861c1589ce02d96f23ad7029fe60190`  
		Last Modified: Wed, 11 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103f5fb6356dce0bb3289f179e8635651d3596f68af9dcec76d316f6e9d43c08`  
		Last Modified: Wed, 11 Oct 2023 07:31:51 GMT  
		Size: 84.1 KB (84097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335fd410bb36645614531f9e7b4f4059ef8f0826221a52bd3b7e7ed298621841`  
		Last Modified: Wed, 11 Oct 2023 07:31:51 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78d7e9e33353646dab930394f9a9a3debe891a8799a23b6faf59bc64eed4ffa`  
		Last Modified: Wed, 11 Oct 2023 07:32:09 GMT  
		Size: 195.5 MB (195463656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23e9b208f6eb4d2fb4a445c28faf334e26005070dc6dd8ac726c3eb8888a0dc`  
		Last Modified: Wed, 11 Oct 2023 07:31:51 GMT  
		Size: 62.0 KB (61980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7709d60cb1c70544f2ba06d28cbc70f937b0990284a5b026acb65cacb194ac7`  
		Last Modified: Wed, 11 Oct 2023 07:31:50 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-jdk-nanoserver` - windows version 10.0.17763.4974; amd64

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
