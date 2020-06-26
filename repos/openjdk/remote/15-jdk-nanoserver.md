## `openjdk:15-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:950a71ed94ab2fb6c4115e5472b32b7cffb0e398adacfa4fe9a3839b2f8d0f17
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:15-jdk-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:bcf2981248ac2bc60567737116e689e58b41b2208a0f301d946bdf75c4dfcd21
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295935644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17674656ab94cc756de851adc3b862014862fd6c86765257b29cf415373fceab`
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
# Fri, 26 Jun 2020 20:06:17 GMT
ENV JAVA_VERSION=15-ea+29
# Fri, 26 Jun 2020 20:07:08 GMT
COPY dir:9e9e711fdce96223607171c03c60a100fb6ddb8f4bf45c421ab27775861f600c in C:\openjdk-15 
# Fri, 26 Jun 2020 20:07:28 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 26 Jun 2020 20:07:29 GMT
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
	-	`sha256:93596b7675c3ff791e648acc77c3a2f01306a9ea5b6f3bdbde96ee861b2e6aeb`  
		Last Modified: Fri, 26 Jun 2020 20:22:16 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8145d3a00cff1f852c86b15f4456e028d29989ac83f6742b61be6d984812d7`  
		Last Modified: Fri, 26 Jun 2020 20:25:49 GMT  
		Size: 191.3 MB (191309949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9fc3010f4cb70b13b6a1ef96e46a06da10908b0eec4fd1d403d3114f07fec5`  
		Last Modified: Fri, 26 Jun 2020 20:22:17 GMT  
		Size: 3.5 MB (3513719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d21959899f6e0ed70a8d0e1c6262c43dace91f8987ce6529d1e5ef9935a422`  
		Last Modified: Fri, 26 Jun 2020 20:22:16 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
