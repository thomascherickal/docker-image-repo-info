## `eclipse-temurin:8-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:293164e1009d484d3897622c24f380ed2fd58952b10a842ab4f798632a26a2c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:8-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

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
