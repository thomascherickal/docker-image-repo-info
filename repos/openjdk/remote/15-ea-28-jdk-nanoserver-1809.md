## `openjdk:15-ea-28-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:3ba3f5c7e9c9b9f191d2a3417781f95cd2d91a9ef8a0c914358f74c8b1896d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:15-ea-28-jdk-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:55f4d73b80e64d7b7cf9e631ae281ba763a73e6f82615009e58fdac6357b3481
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295883943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07554f2467350864b3e61ab23d3eb7cf110bf35ff0a35628b4261d370e5179e3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Tue, 09 Jun 2020 22:42:44 GMT
SHELL [cmd /s /c]
# Tue, 09 Jun 2020 22:42:45 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 09 Jun 2020 22:42:45 GMT
USER ContainerAdministrator
# Tue, 09 Jun 2020 22:43:00 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 09 Jun 2020 22:43:01 GMT
USER ContainerUser
# Mon, 22 Jun 2020 19:25:31 GMT
ENV JAVA_VERSION=15-ea+28
# Mon, 22 Jun 2020 19:26:12 GMT
COPY dir:183d636ef5e35c470f98315e64e2c15b7c8c4ddae84bda358089a01524a8ef48 in C:\openjdk-15 
# Mon, 22 Jun 2020 19:26:32 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Mon, 22 Jun 2020 19:26:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b390ee94e41353252b153770fa99d748992b90bdaf9abf7c785d93be52ee02c`  
		Last Modified: Tue, 09 Jun 2020 23:19:14 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a124a49383ae5eb05208979bcfbadf68055d2672da7f78201fe9a45e8d0bbb`  
		Last Modified: Tue, 09 Jun 2020 23:19:14 GMT  
		Size: 841.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb0c11b8fc0c6457077b02c8314626c0346af177c44a8615448f933e94b909c`  
		Last Modified: Tue, 09 Jun 2020 23:19:13 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29f17e75290909d8f60805f97895317f25ce6c2dc53b1b25e8d6dfe142e6f53`  
		Last Modified: Tue, 09 Jun 2020 23:19:13 GMT  
		Size: 63.5 KB (63500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fe65db6982f49c866229851adc1c64f6e6354b9e0a49d506241693ac2e660f`  
		Last Modified: Tue, 09 Jun 2020 23:19:11 GMT  
		Size: 814.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2291a0b12a6ff271091ffac24a0b53d7ce9e8f02f8ce56d894f9d91379a9ea50`  
		Last Modified: Mon, 22 Jun 2020 19:34:17 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31e1eea87a4ec7631ae0e3cb83cf59af34258afc3a98d11c33ceaf271e77b08`  
		Last Modified: Mon, 22 Jun 2020 19:34:37 GMT  
		Size: 191.3 MB (191267957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4571ef4b26107600e2d6afa0d4fffdb5691b03b64d85a85371176c4adc5e594f`  
		Last Modified: Mon, 22 Jun 2020 19:34:18 GMT  
		Size: 3.5 MB (3504017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2e23677862014e11a7bfe8b8ffd146a571ebe4d5b5d62a9fd4f1b3d3f2381c`  
		Last Modified: Mon, 22 Jun 2020 19:34:17 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
