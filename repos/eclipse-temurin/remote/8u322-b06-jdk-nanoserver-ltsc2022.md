## `eclipse-temurin:8u322-b06-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:4cbb7077cbb545f3cd17c96bb27ec82a62527c7dcfbb828d907802785bc6e3f9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:8u322-b06-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:988e57cfa6ac0dd00c7b6dfea2e01451c66356b9d0a439ef64c21d9f451a8ba7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.9 MB (217944658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdc41ff065d47b8e31233fba5332eed35bcf0947074a75e8062a243b54214bd`
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
# Wed, 13 Apr 2022 15:48:19 GMT
COPY dir:7138e59caf0c25d74e2c65f3638e655f7739a280619af2a4072fd7cd5d6cb20c in C:\openjdk-8 
# Wed, 13 Apr 2022 15:48:30 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:204d0a7cb3c6c113f36542f2c0b5f3d984376b8557128ec32866563e11e4c3f4`  
		Last Modified: Wed, 13 Apr 2022 16:38:39 GMT  
		Size: 100.2 MB (100214242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8457e394eec634ff724f3b4703f29036cf5fe6259c497b0a0c6d9115a72cad`  
		Last Modified: Wed, 13 Apr 2022 16:38:28 GMT  
		Size: 60.6 KB (60618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
