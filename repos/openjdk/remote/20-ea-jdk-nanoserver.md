## `openjdk:20-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:b5de2c1bd46c8c2107d1ea15743c99c7949aa9aaef697b2bb22870b259f6f474
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `openjdk:20-ea-jdk-nanoserver` - windows version 10.0.17763.3770; amd64

```console
$ docker pull openjdk@sha256:4a79d300958ea73ada3e7f4ac9e1630e7ba01a5d7ed8e52b38bc1a676960000e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.6 MB (303553377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d9273437ebf91c95263af099ac8f474ce8eb9409a2be9e8d74fc27c8fc30c2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Tue, 13 Dec 2022 22:53:34 GMT
SHELL [cmd /s /c]
# Wed, 14 Dec 2022 03:06:29 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Dec 2022 03:06:30 GMT
USER ContainerAdministrator
# Wed, 14 Dec 2022 03:06:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Dec 2022 03:06:50 GMT
USER ContainerUser
# Fri, 16 Dec 2022 23:30:06 GMT
ENV JAVA_VERSION=20-ea+28
# Fri, 16 Dec 2022 23:30:23 GMT
COPY dir:f1f409bb958d5b7b7b7cb263a57058fd4ec6eeb2d4125e15e492541e7a995779 in C:\openjdk-20 
# Fri, 16 Dec 2022 23:30:52 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 16 Dec 2022 23:30:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fe06cbef5ac46e54edd743daf1bc2bfa36b294c7ce9104837061c41a4bde7b`  
		Last Modified: Tue, 13 Dec 2022 23:57:01 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8407ccbdbd1b98118842fe985781ff7ccce1a4a02763ce3c7bc5182f0a6cd7be`  
		Last Modified: Wed, 14 Dec 2022 08:49:25 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10a11487b55c583a71e65de52b66756da77520bd91e60c286f53bc275c4776e`  
		Last Modified: Wed, 14 Dec 2022 08:49:25 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b8c7b08a7b6bda536e75dce577a2de479c5b5ac157ae753b5d69a3246b69fc`  
		Last Modified: Wed, 14 Dec 2022 08:49:25 GMT  
		Size: 65.0 KB (65047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410bf6b8361419a87afad95e1191ea2013d36ec41631d7c8a157b17687c9da4`  
		Last Modified: Wed, 14 Dec 2022 08:49:23 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03c0ff74d88cf02aaf2b0e86ebd7f2fcb70c1ebf7b2487f1b725f26ea620c09`  
		Last Modified: Sat, 17 Dec 2022 02:22:20 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508566b26917aafda2a581db1f1c7893bd335af7114ddd751b0b76ac12e4a610`  
		Last Modified: Sat, 17 Dec 2022 02:22:43 GMT  
		Size: 193.0 MB (193037427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a714c7cffff75952682fc574c27ec5999f88380da7995012041269c42922200e`  
		Last Modified: Sat, 17 Dec 2022 02:22:21 GMT  
		Size: 3.8 MB (3772976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5647a85fcbc19d96bc20032e73a5a60c1b23a80844d6fcb2ad8de51a93d04b63`  
		Last Modified: Sat, 17 Dec 2022 02:22:20 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
