## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:ef442447c5b9a6c67452df01998f302c55094547dc46d43bb654d94ccf0af31a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2031; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2031; amd64

```console
$ docker pull eclipse-temurin@sha256:6c4ed1c7cdc6b9606e51bd1d103d7b7e1c54a3ef8ff39224b25d2a1632acf2b3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164161197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0260b5aec5c1f1825fe74acc9abb4fe1a3a4bcf8b7350e86ce2f76cf41dfba2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 06 Oct 2023 21:30:39 GMT
RUN Apply image 10.0.20348.2031
# Wed, 11 Oct 2023 02:14:39 GMT
SHELL [cmd /s /c]
# Wed, 11 Oct 2023 02:16:57 GMT
ENV JAVA_VERSION=jdk-17.0.8.1+1
# Wed, 11 Oct 2023 02:16:57 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 11 Oct 2023 02:16:58 GMT
USER ContainerAdministrator
# Wed, 11 Oct 2023 02:17:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 Oct 2023 02:17:09 GMT
USER ContainerUser
# Wed, 11 Oct 2023 02:17:47 GMT
COPY dir:a0385e93ace109911eb3f9b447c778bc50121e83afa8a78ec38a5f32b2b463cb in C:\openjdk-17 
# Wed, 11 Oct 2023 02:17:59 GMT
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
	-	`sha256:19a659a6819c82d820046e21dc8f4b451012170ce85c646026870c3d99697e82`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f37f39162b0c25f89383c864eff970e2b4d474348c83f10f297506e925beeaa`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb33551667e9e57741cdfc91f6b464adf39fa78ce6d380b810e0c61253726e`  
		Last Modified: Wed, 11 Oct 2023 07:30:59 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d5b0fac9bcddc489ced725a45a3f43c3f60cae734c5b82b37fbc9ed799aded`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 87.9 KB (87919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4834e380ffecef09c287647d524c63045c541ae357d316f993087a6e72a88af`  
		Last Modified: Wed, 11 Oct 2023 07:30:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5f75d8c5be275656d7582e78225b56082e546b96afe9eb8955e9dfe635a796`  
		Last Modified: Wed, 11 Oct 2023 07:31:41 GMT  
		Size: 43.4 MB (43405767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62c166abe4e678d4b5ec25807b076b5abf052935f409cd502f4ab90ebd1cb9e`  
		Last Modified: Wed, 11 Oct 2023 07:31:29 GMT  
		Size: 57.4 KB (57383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
