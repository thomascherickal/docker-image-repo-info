## `openjdk:18-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2ff91223c3630c244ccff5fd325fc79722855240a5c6a2e89c17a8d0e104bc9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2183; amd64

### `openjdk:18-ea-jdk-nanoserver-1809` - windows version 10.0.17763.2183; amd64

```console
$ docker pull openjdk@sha256:bad5d9268f06f41f84ce5c1ec0de032a7d891c62bd8f8ba0a47847897f11db13
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.4 MB (289350531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f46fced82bfa630289c24ad394139fbed911c8c12be3ad352a59ad9ab41cd61f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 13 Sep 2021 03:45:12 GMT
RUN Apply image 1809-amd64
# Wed, 15 Sep 2021 00:38:23 GMT
SHELL [cmd /s /c]
# Wed, 15 Sep 2021 00:38:24 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 15 Sep 2021 00:38:25 GMT
USER ContainerAdministrator
# Wed, 15 Sep 2021 00:38:36 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 15 Sep 2021 00:38:37 GMT
USER ContainerUser
# Sat, 25 Sep 2021 00:19:06 GMT
ENV JAVA_VERSION=18-ea+16
# Sat, 25 Sep 2021 00:19:22 GMT
COPY dir:03acab8d500cdc8613fec84c92f88129bb830a976637f4d3f5bbd90a03295fae in C:\openjdk-18 
# Sat, 25 Sep 2021 00:19:51 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 25 Sep 2021 00:19:51 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3585a81ca503e6c63dce938a5606f4171d7461e51000a92054b3f5692786d6c9`  
		Size: 102.7 MB (102703785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:807d06303c39b2317729754a4c7ad6501e59c16ee464f8f671f9947774f62f72`  
		Last Modified: Wed, 15 Sep 2021 01:10:56 GMT  
		Size: 1.1 KB (1094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353abb4dcfd1456117623d23e4be07d7d5c9e18c7ddea8dfb6225f99efa904b9`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6beb0bff60eb1dfb88e1010454b9aaf8f176f0d004a94fefdedb88d8e7e2a4`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bcb79c10ca3fae0a02ab85be6ab15af3a4ac4d7a0b8b54fd7a9c12cdd0b203`  
		Last Modified: Wed, 15 Sep 2021 01:10:55 GMT  
		Size: 75.1 KB (75126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57b1aff54bbfc95746d48fc4f9d9afbb2f1f02e7d7006d7a7d6265ae52f9289`  
		Last Modified: Wed, 15 Sep 2021 01:10:52 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a081a1465088774817b9162834a893ef6ac96f12eba6642be0391edc7c467919`  
		Last Modified: Sat, 25 Sep 2021 00:32:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6920e4efe22f7bcbde74168c0631dfc7e9b8d93df9700d4d2a627b129df7087`  
		Last Modified: Sat, 25 Sep 2021 00:35:20 GMT  
		Size: 183.0 MB (183041988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42a7103113ad28c11e0600be3a640724a41cf6f45e37c58a8c030cc5af2cdbc`  
		Last Modified: Sat, 25 Sep 2021 00:32:10 GMT  
		Size: 3.5 MB (3523173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5c1135a3b1a344a17b0b93f8173eb9128271f761b457d5c9f64f1967baaa81`  
		Last Modified: Sat, 25 Sep 2021 00:32:09 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
