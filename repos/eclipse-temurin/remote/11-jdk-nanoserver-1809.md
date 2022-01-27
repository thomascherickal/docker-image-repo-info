## `eclipse-temurin:11-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:d8a3c43f5453b5136b211d080ef71d862197f516ccfffc14e03005a40e42f013
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `eclipse-temurin:11-jdk-nanoserver-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull eclipse-temurin@sha256:bf3381e8b97d4a56805ddd8773ade92167ac1922e66a5ade9b0d817908e4af2f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295150114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8071aa54074e48358c1e57e494fe0e473e5079c3f3548bb982a25300212bea0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 18 Jan 2022 01:20:34 GMT
RUN Apply image 1809-amd64
# Wed, 19 Jan 2022 22:25:45 GMT
SHELL [cmd /s /c]
# Wed, 26 Jan 2022 19:15:36 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 26 Jan 2022 19:15:37 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 26 Jan 2022 19:15:37 GMT
USER ContainerAdministrator
# Wed, 26 Jan 2022 19:16:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 26 Jan 2022 19:16:01 GMT
USER ContainerUser
# Wed, 26 Jan 2022 19:16:34 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Wed, 26 Jan 2022 19:16:50 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 26 Jan 2022 19:16:51 GMT
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
	-	`sha256:123ab2ee14a125bf4b0c6cbaa7024d6fd79d88b72564d3f5ffc2a991388ca55d`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22a2e9edcceaff9bcf83e6afe158f5653cb569791bf57461c14bb12dee4c4f4`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd6c39c776fbc28c7dc393f112bb0ec49b97e64c79c5001c3b4c9067461568`  
		Last Modified: Wed, 26 Jan 2022 20:05:11 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5ed98fdccc969f48e18c637043dc0f01001d2592b60ead2a792c7d37dd616c`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 75.3 KB (75305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c4cf8478e4d4c0f8a13f4a6039564552580a3c553158a2405cac2386232588`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f02d23c2d10a747d00a6b7a0e5e13b702809294d12f58f54c9d6776ee2f95c`  
		Last Modified: Wed, 26 Jan 2022 20:05:29 GMT  
		Size: 191.9 MB (191924843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b990ad10118e7f8c6259084d9922c6af0deb76192cc2c2d17548928d8b0ee84c`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 96.5 KB (96480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7e9ed5a78c20ee9aaa8d114201b7782b58e5b36344380adb35c73aa77a50fd`  
		Last Modified: Wed, 26 Jan 2022 20:05:08 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
