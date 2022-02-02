## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:172ef2b5677da0924b8fa240313a05af63d35d154c42a34ff4a0520275df1bd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:891118501b4c0e78656b3b56f5cf9268da7f42efb513308735e54c7e65b46e3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295266003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20a197959bb285585e8f6d7cf0bdac9af1530daba834a31c8d690f69886c301f`
-	Default Command: `["jshell"]`
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
# Tue, 01 Feb 2022 22:32:20 GMT
COPY dir:ca31ccd46ebf34fc51c848053b3110c777231f27811a709a2aa6c558f0ae5c69 in C:\openjdk-11 
# Tue, 01 Feb 2022 22:32:37 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 01 Feb 2022 22:32:39 GMT
CMD ["jshell"]
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
	-	`sha256:97bf04c4512ec584f5db3aba3e22c332fd4d829c825c48fcf28e5eba9c87fa78`  
		Last Modified: Wed, 02 Feb 2022 00:49:54 GMT  
		Size: 192.1 MB (192091313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c71278761ca1b717906e775b675df952175675140931217e4fd83026c65ef8`  
		Last Modified: Wed, 02 Feb 2022 00:46:27 GMT  
		Size: 49.7 KB (49705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f269e2229124e3287603379a8104c5ed41a997a0d447a456b2ef76ff6d9e0f`  
		Last Modified: Wed, 02 Feb 2022 00:46:27 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
