## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:9c6d112d39c983d3b411f117378e0ca5f4c2b3d633a7871b71637f7ced626516
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:2f41f3915656851405423f5215878b5b1975fe90846cf7b1d8d09b43adc01cc8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.2 MB (222237669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f449b7d6135ca7dadb6f30d8af5993bd863ada69a05e03b6f2ae2aa16eb9e0d1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 02:14:40 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 02:14:41 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:14:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:14:55 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:15:04 GMT
COPY dir:809f08e9d949f52aad6441d5338932efbf6208a06192d58db41d3e3c11ba3f9f in C:\openjdk-8 
# Wed, 11 Oct 2023 02:15:17 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:9e573e8d27715408942370bbe3e31eb4ae2c5feadca2cccb3f642115eb3782d0`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a95305dbe93fdf5eb7909af77dfe59c82075bfa61c017c8df26328dfd9e91f`  
		Last Modified: Wed, 11 Oct 2023 07:29:36 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfa1af4fca27ac3e9a84f67da56ec595a2803fbb10b8a798ff27458de06a3f8`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe98fb9ff1cdb5c208cddc16e8f295fc8a2f2c4015171e38254517402041f9b7`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 86.2 KB (86233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a1c6eb49fa819be7d62d2c434696a6dc3cde2b7a8d4494aceae0bc0c7739b2`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4dd5426d5eecf260d703bc49d456e9c3441334540a23c74701626a79a8bf56`  
		Last Modified: Wed, 11 Oct 2023 07:29:45 GMT  
		Size: 101.5 MB (101479230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd440d2da0d1b80c4bc30acfc7c6e70cdd2399fb0b9667a3f8ebcbc44ee7138b`  
		Last Modified: Wed, 11 Oct 2023 07:29:34 GMT  
		Size: 62.1 KB (62101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:d2b842ce979128387707f05fd43c58489d4fe372d05e8e7161394ec68747942d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206100370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cddddb6b6ea40716ad90c62b7964c04cabc57e6c3d43d297f4955cd10a058000`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 01:39:37 GMT
ENV JAVA_VERSION=jdk8u382-b05
# Wed, 11 Oct 2023 01:39:38 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Oct 2023 01:39:39 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 01:39:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 01:39:50 GMT
USER ContainerUser
# Wed, 11 Oct 2023 01:40:00 GMT
COPY dir:809f08e9d949f52aad6441d5338932efbf6208a06192d58db41d3e3c11ba3f9f in C:\openjdk-8 
# Wed, 11 Oct 2023 01:40:12 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:2bfa6f4a1c2a7c533d18ec0dca92bed309d0669d2afab455d6d5212351b975d7`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170446211d70073742ac91df84068c411612746e25962e9ff96b3e9282f20ca6`  
		Last Modified: Wed, 11 Oct 2023 07:20:20 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03792e6d164d8cd335567497987aebb8b5b2425e1cddb7bdb44d32a94149ce4c`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa70d1de1a8dca6152d4582a2933b41dd7345f53273a4973ce1d623209c972e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 68.5 KB (68544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d097244be50912160bdc8158894bd41a8b5cc337313348edc3b35420ac656e`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1a28ac6f682938efb11d62c52c947c7943353b1afcfef288470f6742a36722`  
		Last Modified: Wed, 11 Oct 2023 07:20:29 GMT  
		Size: 101.5 MB (101480219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5631c9fa21ac32ab5ac29148be556756347ccae1fbec09d7500ee00c3a083460`  
		Last Modified: Wed, 11 Oct 2023 07:20:18 GMT  
		Size: 81.2 KB (81233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
