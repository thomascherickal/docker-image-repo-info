## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7b9dc1abce337e900da323c98e8816f4506a8c42d88d8dffa598a88b4a9946d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:7bdc29ed46ad9d11b01887dc63bf983a7aafbb5b0b3a9f89473c72ab03a8b8dd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145930611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37f183869d73fcb69cff50520f2d2b77ce4c3070da201e7b0936b0e674aa10ee`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:31:36 GMT
ENV JAVA_VERSION=jdk-11.0.14+9
# Tue, 01 Feb 2022 22:31:36 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 01 Feb 2022 22:31:37 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:31:50 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:31:51 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:36:53 GMT
COPY dir:37611e99da55cacf359232de16544a31f88bdb2203ee3a1dce3c1fdbd34bf2dc in C:\openjdk-11 
# Tue, 01 Feb 2022 22:37:05 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfb39f38b205ff144dcaeb4c5e7f744d900dcd682628917d87cbcbad236253`  
		Last Modified: Wed, 02 Feb 2022 00:46:29 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78634e061b1d46e5ef6dd4bad558e28dceb0bb5b06db8471ad7001625d32d0c4`  
		Last Modified: Wed, 02 Feb 2022 00:46:29 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ef8b5d13fc7cd97d2b50d7b002f55a6145054dd3f7b3b7c1a4371f3e0e0f9e`  
		Last Modified: Wed, 02 Feb 2022 00:46:29 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cfe1edcab6069e4fc9d8bbb8490cff0adfee4d75a0c32d45cf276ac27e87214`  
		Last Modified: Wed, 02 Feb 2022 00:46:27 GMT  
		Size: 71.6 KB (71562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:583fdb7547f83f9a55f711ced1d7d61f55d9f48d50fceb28c2d5e0739e0032de`  
		Last Modified: Wed, 02 Feb 2022 00:46:27 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650bac854367f5cd85cc5c666cfbd27e5b92c4785e472988744309da77efb4b2`  
		Last Modified: Wed, 02 Feb 2022 00:50:55 GMT  
		Size: 42.8 MB (42757807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8124612e6e2cf490274cfeb0cec00740961824c566efd4fb77c3d82df6eaf26`  
		Last Modified: Wed, 02 Feb 2022 00:50:46 GMT  
		Size: 49.0 KB (48987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
