## `eclipse-temurin:8-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:fc4633d4936591baa04f27a9a287e0e76d768b9c7b3d6e005cf01815a41066c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8-jre-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:313c04fd194a5c89bc2b9a616b5ae859dbdd22384bb8ebdcaa856be0c90ec0e2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142317989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a870b8411bdec4c0326680fe39dbd9a6f49bbb3b6dbb6f37e9744c636fde111c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Tue, 01 Feb 2022 22:20:19 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Tue, 01 Feb 2022 22:20:19 GMT
ENV JAVA_HOME=C:\openjdk-8
# Tue, 01 Feb 2022 22:20:20 GMT
USER ContainerAdministrator
# Tue, 01 Feb 2022 22:20:38 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 01 Feb 2022 22:20:38 GMT
USER ContainerUser
# Tue, 01 Feb 2022 22:25:53 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Tue, 01 Feb 2022 22:26:04 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:b5c97e1d373f591225559869af7f4f01399c201f89d21f903b1d23c830aa0a3f`  
		Size: 103.0 MB (103046552 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a1b3e13bb7b3d4b61b5f49a91d6eb9bfcf5539ab89c3687d608f17713c2409b5`  
		Last Modified: Thu, 20 Jan 2022 02:21:30 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e78c8a17b181b5ee6535c053d3b2c85650f349734b9858cef8526bb76643c9b`  
		Last Modified: Wed, 02 Feb 2022 00:42:33 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710ff6b075e15cfa0c71db2df68e9ba3d9dcaee6f30846fb65cfa9384800f680`  
		Last Modified: Wed, 02 Feb 2022 00:42:33 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef71c6d2d842ce5e520afb93ba595f86d312e6716a10b39dda8c91d930745fff`  
		Last Modified: Wed, 02 Feb 2022 00:42:30 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e936d7e60e98bf322a916bcb76ac03d1afcdbd0cd4044bfd51f639763c1fedbe`  
		Last Modified: Wed, 02 Feb 2022 00:42:31 GMT  
		Size: 71.0 KB (71002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abbf95538367cd4deb8ae9bfb78a1316ae4e8e1b74132b309bdf80cd83f3156`  
		Last Modified: Wed, 02 Feb 2022 00:42:31 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae78fc6a5a7b58e5b19bd563f733a04b7150875b6829b87ad80fd5463a22d271`  
		Last Modified: Wed, 02 Feb 2022 00:44:48 GMT  
		Size: 39.1 MB (39112282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49201bb427a665882e7eef39ddd36f145071ed41e613d3faf726ec476c62139`  
		Last Modified: Wed, 02 Feb 2022 00:44:05 GMT  
		Size: 82.4 KB (82416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
