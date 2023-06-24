## `eclipse-temurin:11-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:398b782cd0170b604ebb163761f854e5f0038cef9b07ea2611bb12461e3fb8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:11-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:46f4833cd2a1eab9e11a0a55d252207bc9925da4850f57e64bc022f4c09fa897
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.3 MB (163335768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b361c9ff3a7380978a7c75b8232d9c5374129e97ae8db8864c4500b5bfbd55c4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:09:40 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 01:09:41 GMT
ENV JAVA_HOME=C:\openjdk-11
# Sat, 24 Jun 2023 01:09:42 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:09:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:09:53 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:10:41 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Sat, 24 Jun 2023 01:10:55 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71328532fe3e7c9a5b123f73fd88dd66aed81951658212fa82c3f81ad09e1fa5`  
		Last Modified: Sat, 24 Jun 2023 01:35:13 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7254d80ed10cf22be8ca4b228566a08f2f74518f7e577779370cd662465b5`  
		Last Modified: Sat, 24 Jun 2023 01:35:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613dec9326bb21840e70e24320ff7edfa56e82381e34835a27c01969e463be7`  
		Last Modified: Sat, 24 Jun 2023 01:35:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02161c0d2c1a9ef9543954f1fb02a00b48ee2878872ed645cfc6b62e70ce70e`  
		Last Modified: Sat, 24 Jun 2023 01:35:11 GMT  
		Size: 75.9 KB (75945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7368a12cc6a47c7ca5060834684282b674bf3c5ffb1cdb6f3f4a1a06d13db9`  
		Last Modified: Sat, 24 Jun 2023 01:35:10 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01617b8f08e848aba8f79b3dc2068229dc4c89e643464856642d5426f1c6d01c`  
		Last Modified: Sat, 24 Jun 2023 01:35:48 GMT  
		Size: 43.2 MB (43164163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ea723f8afbe4c58b0f9e08e2ffaeb9607cd49e61d4917ed20368c8c21fca3`  
		Last Modified: Sat, 24 Jun 2023 01:35:40 GMT  
		Size: 61.6 KB (61614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
