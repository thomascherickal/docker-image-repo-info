## `openjdk:15-ea-31-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:5df8506d0930fb0d6a0535c935eed1896234d34c3c421396928edf1fe92e01ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:15-ea-31-jdk-nanoserver` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:73a614efdf3ecf9e60bc200fe131fc0f3d8e78db6fa520c7ae34eec75c066cc7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295958923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bb30e951a0866bb15ab160ca08bba38f01187d6e335d436c07274d70fcd293`
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
# Fri, 10 Jul 2020 01:25:53 GMT
ENV JAVA_VERSION=15-ea+31
# Fri, 10 Jul 2020 01:26:37 GMT
COPY dir:8c9ba2918e3c2737605432ccf9b34e043f1efb82354836eddf5cf3bbad167ed1 in C:\openjdk-15 
# Fri, 10 Jul 2020 01:27:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 10 Jul 2020 01:27:04 GMT
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
	-	`sha256:3826d184f72f4e6dbca328126c573260538df2241c317f6f25bf4904be6ed81d`  
		Last Modified: Fri, 10 Jul 2020 01:35:05 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dab88c8b5a0caf03f20646349c03cd0a1c245c8c901408dd96c9f7fe5b3be3`  
		Last Modified: Fri, 10 Jul 2020 01:35:25 GMT  
		Size: 191.3 MB (191332778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8127baf13238bf9f5f8ce1a44b53e78b8814b0c7b6ea3036bf5e3d61f50dce3`  
		Last Modified: Fri, 10 Jul 2020 01:35:06 GMT  
		Size: 3.5 MB (3514191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90f18f9dc88d23d334ef04d46e75912644eabf542c39b5fb8b66e033d4ec345`  
		Last Modified: Fri, 10 Jul 2020 01:35:04 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
