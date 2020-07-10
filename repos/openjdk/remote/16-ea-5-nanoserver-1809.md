## `openjdk:16-ea-5-nanoserver-1809`

```console
$ docker pull openjdk@sha256:176299f22986dc87d58db4118623a7c774892bfa2ee7f0c21d5858eeb73c3b41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:16-ea-5-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:a9d9795ae326af91c09cb5c33f92b16350178a027f9cf142dd5f87e417a0c32b
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296570773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5735281d7ec7f70821fceb5229e5273fd0247547243cb57935cad148048b390c`
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
# Fri, 10 Jul 2020 01:19:28 GMT
ENV JAVA_VERSION=16-ea+5
# Fri, 10 Jul 2020 01:20:21 GMT
COPY dir:ab91ee3bf26eda34a581e70062adc4a24889abc64f935e4fe64edf4b7fd621b4 in C:\openjdk-16 
# Fri, 10 Jul 2020 01:20:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 10 Jul 2020 01:20:39 GMT
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
	-	`sha256:d0b6c7c5ac15063b47fc1e31f95b2ad50124b8fd7cfc22f984dd796c16d4cf24`  
		Last Modified: Fri, 10 Jul 2020 01:32:59 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb38d47d8245ce12574b38a8227bca895e224d6a09f038dade153af728da253`  
		Last Modified: Fri, 10 Jul 2020 01:33:20 GMT  
		Size: 192.0 MB (191971217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58a39c667add6050e3af655c35049e209267cb90f9bdc01f0a8290bc41ed9f6`  
		Last Modified: Fri, 10 Jul 2020 01:33:00 GMT  
		Size: 3.5 MB (3483678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c149544030474b39d7052b8df13ea0d4fd09ceb333f2c72c11ef9a396762d2c7`  
		Last Modified: Fri, 10 Jul 2020 01:32:59 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
