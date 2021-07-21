## `openjdk:8u302-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5859132970badc7c78ab41228b9bedac15e017ccf05bc4b601cfaa3f029c3347
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `openjdk:8u302-jdk-nanoserver-1809` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:f0171d834eb9151f030b955a709be906a40bff26320d0eb5440ea030c6ab341c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.9 MB (203940193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ef1df3ab5cfd65ebf2afccabe10dfe21ab65904a8b6b529e0e3444d2ef45f2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:53:30 GMT
SHELL [cmd /s /c]
# Wed, 14 Jul 2021 03:30:22 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 14 Jul 2021 03:30:24 GMT
USER ContainerAdministrator
# Wed, 14 Jul 2021 03:30:39 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jul 2021 03:30:42 GMT
USER ContainerUser
# Wed, 21 Jul 2021 18:29:42 GMT
ENV JAVA_VERSION=8u302
# Wed, 21 Jul 2021 18:29:59 GMT
COPY dir:82904e6295068720536f940f57626186b2820e368b810e639bd5a3957d468086 in C:\openjdk-8 
# Wed, 21 Jul 2021 18:30:18 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d8754fb12dd351c91bed29d92c703cddb135a78d8f056b6a3bf13a251c1d2d`  
		Last Modified: Wed, 14 Jul 2021 03:42:27 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3609dce65084314b4fcdbee2b4c9cac86e4ba6a2f6731228036cb6d732decda9`  
		Last Modified: Wed, 14 Jul 2021 03:58:13 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea74f08cf2d09382b86b1680d8741d756d6136a94cbad80c4521348f4999d4`  
		Last Modified: Wed, 14 Jul 2021 03:58:13 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a284e1f3d144cb79b4c435ae2a981fcfdb8c8dc7e29dc1a4ca3fc1df81e5ff`  
		Last Modified: Wed, 14 Jul 2021 03:58:11 GMT  
		Size: 67.4 KB (67382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501cb4cf39ea8969b47e4aec6a12c620974aefe7be361eb0a17f5cd081fbeb90`  
		Last Modified: Wed, 14 Jul 2021 03:58:11 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d0cc08063bee25d8049ae3e8e0d938ae3ac805bc9d8f8c912494a8daf08a63`  
		Last Modified: Wed, 21 Jul 2021 18:44:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5dc21bff0ddd68087cb30e76249b76c0c32143efdbcf5e8a3bd70e83c4b13b`  
		Last Modified: Wed, 21 Jul 2021 18:44:37 GMT  
		Size: 101.1 MB (101052275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59692407a2815454ea01529526dd85aeb2bf1bead22bfb9ec43ef7e3fb86c578`  
		Last Modified: Wed, 21 Jul 2021 18:44:24 GMT  
		Size: 89.1 KB (89146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
