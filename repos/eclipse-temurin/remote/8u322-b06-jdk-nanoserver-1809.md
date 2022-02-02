## `eclipse-temurin:8u322-b06-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:f9ff4fdf8d7750338c1aa3e331aea207fe8e118796752fb5f9bf1b46fa7731e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:8u322-b06-jdk-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:dc3a7877300941c5cf9e6fcdacb3689fb9e99a6935252585b8998a508df82f55
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.4 MB (203422104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304f12445a72a8eeda3df5613785c6876e535b1ba15ab1ccf786e9fd3ae2ba8b`
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
# Tue, 01 Feb 2022 22:20:52 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Tue, 01 Feb 2022 22:21:06 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:2c17f36cfd73c0283533e75edecb8cc02aead4c781f282482e614de74242b6f6`  
		Last Modified: Wed, 02 Feb 2022 00:42:43 GMT  
		Size: 100.2 MB (100215926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b15b7ec2219bed45f7a9a4ba6d0fd78e1e3daf29c121793e696dd949fb0947`  
		Last Modified: Wed, 02 Feb 2022 00:42:31 GMT  
		Size: 82.9 KB (82887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
