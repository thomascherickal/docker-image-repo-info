## `openjdk:16-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:cfe0c39e40b792996fb979a173432d2d3054e70d25fc55d546485d848d5571e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:16-ea-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:ee19899ff1bbf0e5345ec2369644eeb88afde1f35178ab01067ae0d237eac1a7
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295972526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f86a8e3bdb4d52da470f593f0ddee82f4c44a62214fa7305657eb18ed6e5b7e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Tue, 09 Jun 2020 22:42:44 GMT
SHELL [cmd /s /c]
# Thu, 18 Jun 2020 21:20:54 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 18 Jun 2020 21:20:55 GMT
USER ContainerAdministrator
# Thu, 18 Jun 2020 21:21:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Thu, 18 Jun 2020 21:21:11 GMT
USER ContainerUser
# Mon, 22 Jun 2020 19:19:25 GMT
ENV JAVA_VERSION=16-ea+2
# Mon, 22 Jun 2020 19:20:16 GMT
COPY dir:b3609f1221d7270c026c719a55fb40328a50f0fbf423adb5e33f5eb9593e5cce in C:\openjdk-16 
# Mon, 22 Jun 2020 19:20:36 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Mon, 22 Jun 2020 19:20:37 GMT
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
	-	`sha256:6735890902f0d30df68ef896ea73cd7d60bdd05747cff4957193c1e609fff89a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee48b3407ba988368d7894a7733194fa4aa014b7f58f2d8c7fcaef8e2671a28`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6045b891a8218b59a2fddf2b6cac14838a3415c9d2d3092bc26b5e034902d9a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 67.2 KB (67242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f442edf533cb5c66c3872015a3894f657674d730051b398dd331afcfe90617`  
		Last Modified: Thu, 18 Jun 2020 21:28:18 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab57a62be2ec6eaa4cb79528f29cf568f06cf483a93aa098e9d3c446a69139`  
		Last Modified: Mon, 22 Jun 2020 19:32:12 GMT  
		Size: 861.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7662ab41a67beedba5e13a7beb4e0c81f18717cf878917fd85e1e96696391bff`  
		Last Modified: Mon, 22 Jun 2020 19:32:32 GMT  
		Size: 191.4 MB (191374463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2fbf38583a20b808adf10791632184f9125652d5d9629c7be0b44c6eb21ff3`  
		Last Modified: Mon, 22 Jun 2020 19:32:16 GMT  
		Size: 3.5 MB (3482237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592d9b413303ae34ac1fc10c03f8e8405e2044d26632ced817eab3622e57fc1b`  
		Last Modified: Mon, 22 Jun 2020 19:32:12 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
