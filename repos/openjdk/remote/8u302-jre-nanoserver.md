## `openjdk:8u302-jre-nanoserver`

```console
$ docker pull openjdk@sha256:845115eca2988891be1150596908aea40672f0ff29b0db1c614e3a1215da306e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `openjdk:8u302-jre-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:7d4805aaec8c2453f31c86ff0faf021fb062922fbbed7d2ebf81ef0e9d6e254d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141100424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:073a9b4364dc997ebc0d66d746127dd09f34752851dbb8b89f741a6f96718fac`
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
# Wed, 21 Jul 2021 18:33:55 GMT
COPY dir:58006f68c4ea109e560c76de14918bddd55bac9724011203b6cdeb031fa20971 in C:\openjdk-8 
# Wed, 21 Jul 2021 18:34:12 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:847782a71b107b4bb02d88e5b015af4caa5a86182df3b8d6583712f8e736296e`  
		Last Modified: Wed, 21 Jul 2021 18:46:57 GMT  
		Size: 38.2 MB (38221993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fbd595c1fc7055c32a0d12d1593fcacfa15dc23588d097122b9ec4170a7c98`  
		Last Modified: Wed, 21 Jul 2021 18:46:51 GMT  
		Size: 79.7 KB (79659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
