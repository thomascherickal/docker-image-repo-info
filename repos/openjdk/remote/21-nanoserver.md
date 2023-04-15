## `openjdk:21-nanoserver`

```console
$ docker pull openjdk@sha256:e6b0f161718b0735de9f48dbfab436a84cb8ce17a64d9ba0f4b48e0b1183aaa0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `openjdk:21-nanoserver` - windows version 10.0.17763.4252; amd64

```console
$ docker pull openjdk@sha256:9b1517c29013f66fe94b375f7e2eedcdcaeb22e317b6b72dce1673f0b5c56322
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.7 MB (306720867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6ca66c4adfeb02ee517deda43b687cbaad18c223cd0cdaf707051cc398b0a73`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Tue, 11 Apr 2023 23:45:42 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:45:43 GMT
USER ContainerAdministrator
# Tue, 11 Apr 2023 23:45:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Tue, 11 Apr 2023 23:45:57 GMT
USER ContainerUser
# Sat, 15 Apr 2023 00:25:42 GMT
ENV JAVA_VERSION=21-ea+18
# Sat, 15 Apr 2023 00:25:56 GMT
COPY dir:c22769a345a5fcbde3eab8b8ffec1a842f4ee8370e025ab0683c358637b2f099 in C:\openjdk-21 
# Sat, 15 Apr 2023 00:26:14 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 15 Apr 2023 00:26:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959014ae4c354475658573dc2e10e98575d191deef98e1f23bf7cb9f4768408f`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b662327c70093bac13b7d07354fdbcd6967cbc13aaac870ca2e077fafefceb8`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9446ad09d009884e8a1db2085ef50cd6467dc3270eca7bac27fca70698013943`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 68.0 KB (68014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1335b1a9f9197626e9424d9d24737142c9d98659cc7f5510ca10378488d00b51`  
		Last Modified: Wed, 12 Apr 2023 00:52:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765fac772c4668c0046814b62845bcbff4f49644281307e176f811293e286ce0`  
		Last Modified: Sat, 15 Apr 2023 00:28:13 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a650dcad8be28d942a58f24a378bdb4705dc71f70dbaaf371f9e9ec8f2357390`  
		Last Modified: Sat, 15 Apr 2023 00:28:32 GMT  
		Size: 196.1 MB (196085231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09512e6f23b14f73935306a1d644134a48ae38f1f13c7d351aac6a98256d3195`  
		Last Modified: Sat, 15 Apr 2023 00:28:14 GMT  
		Size: 3.8 MB (3771788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7ec1c7d6ef7c5110971b43060eafb24e2df23cd4a4fd0e67ee67c38807b6ef`  
		Last Modified: Sat, 15 Apr 2023 00:28:13 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
