## `openjdk:19-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:1a9f29852f662ab5b0b880e80cde0ef8f4f09547939de7dc1b43ba57f7c7cafb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:19-ea-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:10822861a942e57eb3c39ed7768636d63508ddc9e8034cce5131353bb44ec933
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.3 MB (291333309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f967a1f116eb19b5e399cdb8730d39477475f8b3cdc3d69bebe799b250cc4ec0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 05:18:44 GMT
SHELL [cmd /s /c]
# Sat, 18 Dec 2021 07:02:53 GMT
ENV JAVA_HOME=C:\openjdk-19
# Sat, 18 Dec 2021 07:02:54 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 07:03:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 18 Dec 2021 07:03:07 GMT
USER ContainerUser
# Sat, 08 Jan 2022 00:50:38 GMT
ENV JAVA_VERSION=19-ea+4
# Sat, 08 Jan 2022 00:51:10 GMT
COPY dir:0e17b3361127d84da6697596100040ca0746296f166480523a243817ad096d15 in C:\openjdk-19 
# Sat, 08 Jan 2022 00:51:31 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 08 Jan 2022 00:51:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4c557aac927613dd487d7c04b01a8eeb8ad174693f61b14c8f4285f1db6afdd2`  
		Last Modified: Sat, 18 Dec 2021 06:13:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee77840953b5908197d8833c877fc68713477ba9d823d0917d99682670f0a3f`  
		Last Modified: Sat, 18 Dec 2021 10:56:34 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0e4c6e5345c964ccca26a0985b4ee9da30d0ef03b76b305170b194938512c6`  
		Last Modified: Sat, 18 Dec 2021 10:56:34 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed1fe46a03128a021a9357486f07c8e6f1d8237ed48f484797f70e45efcc27b`  
		Last Modified: Sat, 18 Dec 2021 10:56:33 GMT  
		Size: 67.4 KB (67397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0a3a92f853e640905ade39909c46ce2b476df94464a7649628a0d6a22118db`  
		Last Modified: Sat, 18 Dec 2021 10:56:31 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aaa8ba18b8005eb5c4b67cc71c526b7ca8033d67d06ae061b2861365f4b5fad`  
		Last Modified: Sat, 08 Jan 2022 01:09:07 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c2b321d421404c492693cfc048e2492d6c329860ed88c650095eef3e6f67c3`  
		Last Modified: Sat, 08 Jan 2022 01:09:28 GMT  
		Size: 184.8 MB (184807550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdab734af554fb366a747192be1aea56d7d99edc7d8af5b37937019297d800de`  
		Last Modified: Sat, 08 Jan 2022 01:09:11 GMT  
		Size: 3.5 MB (3547419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697a4ab71bf95dc87f8a2e8b8eb4c817f4f07b325c1ac2922b43f46765fb6a28`  
		Last Modified: Sat, 08 Jan 2022 01:09:07 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
