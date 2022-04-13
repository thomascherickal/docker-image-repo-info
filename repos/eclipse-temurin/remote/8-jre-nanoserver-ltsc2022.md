## `eclipse-temurin:8-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:f14640550d71aeb836e7d33c6bdbc6591569c571d0e3e76b181bbb43ec113779
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:8-jre-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:24689e8feb18dfe2072713d189fdb949ada7cd7d30bfbfc1d5a8def6c6e499f2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.8 MB (156839158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76ec4c27adce3cc6119824179c378490faa6d89ea3da9db4b4f7196ae65ef55`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:47:59 GMT
ENV JAVA_VERSION=jdk8u322-b06
# Wed, 13 Apr 2022 15:48:00 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Apr 2022 15:48:01 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:48:09 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:48:10 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:48:40 GMT
COPY dir:d1a6722e8aa7d48dd5f1c45f802460fd028688b69665fdd4cb7519baa4fcb589 in C:\openjdk-8 
# Wed, 13 Apr 2022 15:48:50 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:924a7c42e559a85c0bc74dbb028ddeee43fe67b0f59c81c60cbda0082e0e3ae5`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165c132f9b7a99d82c74c6e8ae2683134d8e6f6668c194c6d67227d4f15f0921`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.1 KB (1089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be478e3d24da72d6160915d7d5d8cf5a0eab20bcbb291144533fc87aaa32f0d4`  
		Last Modified: Wed, 13 Apr 2022 16:38:30 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a40a1449530555cd30b19c0d58a8e8e0938e6bf3f12ef294d872872114d4fdc`  
		Last Modified: Wed, 13 Apr 2022 16:38:28 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7e54c826a7bf34947d87d543ed9b1b357b3c724a7b29bbb32d5c4d4126874f`  
		Last Modified: Wed, 13 Apr 2022 16:38:29 GMT  
		Size: 85.1 KB (85101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed1f47e5ce93097a6029a4c86ff2abc093cb444ec2ba87a93842307b0aa671c`  
		Last Modified: Wed, 13 Apr 2022 16:38:28 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69b7ccee87a15e8a0c8ec5b5a409d033694d71fcfdafda90ba6ed20f5cdd7d2`  
		Last Modified: Wed, 13 Apr 2022 16:39:34 GMT  
		Size: 39.1 MB (39107985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ccc35601dbd3f04f5e037bdca83dff81eb4c175860f1866833518f5abe7cb2`  
		Last Modified: Wed, 13 Apr 2022 16:38:53 GMT  
		Size: 61.4 KB (61375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
