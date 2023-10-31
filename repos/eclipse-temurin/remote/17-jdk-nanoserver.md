## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:154fefbf3d9782e0aecd3b95b5209916b2d8386033dc66b001f57d14d7e7c130
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:fb14e112899f7a7b8c352bef52664f8a468606fa450eab75ac24d01a62d6083d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.4 MB (307411025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6565eb995073c5bcc4b04806c9f1a67a2269fd3c73735e74bb9a8c29af56190d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:43:04 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:43:05 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 30 Oct 2023 23:43:06 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:43:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:43:14 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:43:27 GMT
COPY dir:abd8f71dbffdebb78ff7b01992fc9930e8aa0c6f2b1d8e6ad05b2a0c8da5ed1e in C:\openjdk-17 
# Mon, 30 Oct 2023 23:43:38 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 30 Oct 2023 23:43:39 GMT
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
	-	`sha256:9ceba97b8485afc5e3ccc0c0a5abac686418cbb3abf82ac9c9a3f4e08abd236b`  
		Last Modified: Mon, 30 Oct 2023 23:56:40 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a12a64c77e447f09b8ebde533756258f45b31c680ae4b3b6ea0c907c1cd521`  
		Last Modified: Mon, 30 Oct 2023 23:56:41 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6b06cd8393c6eec6d614e54464d194cbfa583eda3eb6e3ec2d858b8d2a301b`  
		Last Modified: Mon, 30 Oct 2023 23:56:40 GMT  
		Size: 1.1 KB (1099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35031c8b7bf4e44443217a239a627dffa4374aeff8c763cefcdf4dcecabe5df9`  
		Last Modified: Mon, 30 Oct 2023 23:56:38 GMT  
		Size: 79.5 KB (79532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abd0553f037e2beb50c30f9fba77cde9299e080b7086825969fc378b254157a`  
		Last Modified: Mon, 30 Oct 2023 23:56:38 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f517d05bba9881e7fd5008934fc2bc281a78939840be23f12e446ee5ba796c1d`  
		Last Modified: Mon, 30 Oct 2023 23:56:56 GMT  
		Size: 186.7 MB (186659311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2212e7e52ed65c5757042bf098ef94ef7867c643d4893f8fd856677b05d9aaea`  
		Last Modified: Mon, 30 Oct 2023 23:56:38 GMT  
		Size: 61.1 KB (61096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aedc8fe2611e27434b2cb51899b54e4bd528385e8e98f06f0df142eb6ea5487`  
		Last Modified: Mon, 30 Oct 2023 23:56:39 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull eclipse-temurin@sha256:5d83182fd4c5421506276c87e71f2d0be39a23e60a1f92235b49c2752538e645
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294795960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2305c51bf4aacc587b878e6e48ef095a3e82e407f64e5d3234d2a4d065a6b4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 01:39:37 GMT
SHELL [cmd /s /c]
# Mon, 30 Oct 2023 23:28:40 GMT
ENV JAVA_VERSION=jdk-17.0.9+9
# Mon, 30 Oct 2023 23:28:40 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 30 Oct 2023 23:28:41 GMT
USER ContainerAdministrator
# Mon, 30 Oct 2023 23:28:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 30 Oct 2023 23:28:48 GMT
USER ContainerUser
# Mon, 30 Oct 2023 23:29:01 GMT
COPY dir:abd8f71dbffdebb78ff7b01992fc9930e8aa0c6f2b1d8e6ad05b2a0c8da5ed1e in C:\openjdk-17 
# Mon, 30 Oct 2023 23:29:14 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 30 Oct 2023 23:29:15 GMT
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
	-	`sha256:544ee40eb274d2cf11d28d99d0c8494a24e00f0f1137b7e564be49e87156f107`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161906f3b49bd6fd6c057a7ab136803617df69e360227bf85071954cbaff5bd`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9577e25e1dd402829dc73e75680c93ecc3ab8b98e0ab4a0426d280e445f0b3dd`  
		Last Modified: Mon, 30 Oct 2023 23:51:29 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8466f9d333da539e80924cc14314d112e43eba15e91d933a916db00a4544c4ba`  
		Last Modified: Mon, 30 Oct 2023 23:51:27 GMT  
		Size: 68.3 KB (68304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8ac5c462e2a023aec1e4bc0979a6aca435b4e18a061c38f710d3ba7720f7a`  
		Last Modified: Mon, 30 Oct 2023 23:51:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20872b982a4cc7310b606d224997a4fcfa6239a2e7b14c0d47c9d6d1fbfc565`  
		Last Modified: Mon, 30 Oct 2023 23:51:44 GMT  
		Size: 186.7 MB (186659481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b3f3723105da23eb859e3222177c0e220700920e6220ee8ad41aaa3faf3f17`  
		Last Modified: Mon, 30 Oct 2023 23:51:28 GMT  
		Size: 3.6 MB (3596725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9645f4d6ce6ce3c44561378d2db5c09ccc846b94b3b6a598085f0af2f6f2535`  
		Last Modified: Mon, 30 Oct 2023 23:51:27 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
