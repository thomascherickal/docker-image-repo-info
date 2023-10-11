## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:25d4276a226b90144cb828a60ffaf82333ed8a209b9c2d3bda7d63d70f57fbec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:2b77c5ca1784b9794910ee1529938c7ceeca96ea474d9f3cd2e589f0d325ed9a
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163970362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:141ebec29c16b3960c45f3e6553552ed0382a77a2846f65c4e06cf9539616173`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:15:48 GMT
ENV JAVA_VERSION=jdk-11.0.20.1+1
# Wed, 11 Oct 2023 02:15:49 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 Oct 2023 02:15:50 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:15:58 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:15:59 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:16:39 GMT
COPY dir:8fefe94e6208edfa85d9fa21e3e899009fbc5498c10b88818044df54f9a7b652 in C:\openjdk-11 
# Wed, 11 Oct 2023 02:16:50 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:ca5b30c660e7f95ab2f09973c8367da0af150cd9e09bee428e61415cbeafef83`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99da9dc14e7b0500712ab9187495d6098529b4967951b59228b07afb096df440`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02f7922ddee5615f25e8c52c728cc5f139aac0be11956f7a7d0074c3747968`  
		Last Modified: Wed, 11 Oct 2023 07:30:13 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6eb8225ff2b985a7ecf4ab61f0858e37359afccb00bb112e6ffc485cf72b5fc`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 79.6 KB (79631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dda70c55c8e83cc305bb2d3765daaf5a54aec316b3aff8d16c649e19f7c1cf`  
		Last Modified: Wed, 11 Oct 2023 07:30:11 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c301d1db0ebd5a1fb4aa6b10a2a3796620d25b47c7c46c0d3977c37660c11f70`  
		Last Modified: Wed, 11 Oct 2023 07:30:48 GMT  
		Size: 43.2 MB (43218537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f895b2c0e4dc1c88186a3ab127da567a10b39903291aeaf33a6191fa322ae`  
		Last Modified: Wed, 11 Oct 2023 07:30:41 GMT  
		Size: 62.1 KB (62105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
