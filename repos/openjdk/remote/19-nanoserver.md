## `openjdk:19-nanoserver`

```console
$ docker pull openjdk@sha256:990d91f0a33a054daf76b9680aae04f02abd79af1abe96dbb4172dbade4caffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:19-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:95354f9947f158fbdb2c4dff9b7bde6f2e8bef25164917b18acabfab8edc21a8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.3 MB (291314407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e060e4e977aa6292dc95a003f0ecca5963dea04205679b45c5170f5e96c8066`
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
# Sat, 18 Dec 2021 07:03:08 GMT
ENV JAVA_VERSION=19-ea+2
# Sat, 18 Dec 2021 07:03:25 GMT
COPY dir:bd7bc461b48bb9179e5516b6f1130fc1f6dd73f65463cfeb9c9ce02d9203c5df in C:\openjdk-19 
# Sat, 18 Dec 2021 07:03:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 18 Dec 2021 07:03:39 GMT
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
	-	`sha256:b1df1209406f54c6bc5c50198be6576ea0081794c633a4ab3bcea11c1789ad31`  
		Last Modified: Sat, 18 Dec 2021 10:56:31 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207fb1d0806998ef564816fb653ada43cf68d79b23a2afe9c3911010645a478f`  
		Last Modified: Sat, 18 Dec 2021 10:56:51 GMT  
		Size: 184.8 MB (184796989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8147719e00410774a2d1a0e64317872f0481e851a6586c1b5132710642d6925f`  
		Last Modified: Sat, 18 Dec 2021 10:56:32 GMT  
		Size: 3.5 MB (3539009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0639daa6925e811773185ca4a2f5120a5c9d8afcce722b9591b91435b3cc67d1`  
		Last Modified: Sat, 18 Dec 2021 10:56:31 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
