## `openjdk:16-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:e93fabb6c45817244dbfa4c10dc9e6f22d54dc2b2d1d36c6a71b64308cc1871a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `openjdk:16-jdk-nanoserver-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull openjdk@sha256:9fa919d96e64c92e7580308c910f2f28cf30fc3562011f2fb42d5ce8047a59ea
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297066861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f63522c6e221bb616e983a4599409a2b2faf320a9eb706731c36f32e877fe1a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Sep 2020 12:08:18 GMT
RUN Apply image 1809-amd64
# Tue, 08 Sep 2020 20:13:38 GMT
SHELL [cmd /s /c]
# Tue, 08 Sep 2020 20:13:38 GMT
ENV JAVA_HOME=C:\openjdk-16
# Tue, 08 Sep 2020 20:13:39 GMT
USER ContainerAdministrator
# Tue, 08 Sep 2020 20:13:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 08 Sep 2020 20:13:54 GMT
USER ContainerUser
# Mon, 12 Oct 2020 17:19:17 GMT
ENV JAVA_VERSION=16-ea+19
# Mon, 12 Oct 2020 17:19:56 GMT
COPY dir:bdf4e5ef39680bc6900a8942c0e86a2fa60a3a2a7434c43c49d0857baa5ba447 in C:\openjdk-16 
# Mon, 12 Oct 2020 17:20:24 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Mon, 12 Oct 2020 17:20:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ecf9bb62dc6eedea9fd367628f8715dea75b7d2053afa4b5121e7809aa692139`  
		Size: 101.2 MB (101239122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f72ec155bceaba8b4a5cdbd7aa79586c7296a801af5364a691c46191c910e2da`  
		Last Modified: Tue, 08 Sep 2020 22:29:01 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b2192657885f813dd6fa78d8ba65d02e35934c0c45121f5cb3004298998876`  
		Last Modified: Tue, 08 Sep 2020 22:28:59 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe914594cd5b7b9a0b5c0080fe6c643b51eecedb3197955dbea30a0005a9132`  
		Last Modified: Tue, 08 Sep 2020 22:28:59 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dc65079aab4e95e3a823193385145a250bbb9e13cd9c5e02a35844069217`  
		Last Modified: Tue, 08 Sep 2020 22:29:00 GMT  
		Size: 65.1 KB (65142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bee2eb45cc55aae1760d1937d9de7b70abd95c9488b97a8288d08b472684fb5`  
		Last Modified: Tue, 08 Sep 2020 22:28:57 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b912509ec6f0bc45cd6525c33a8bb3a4aa27e227a3943e38964272cc8f0e8a2f`  
		Last Modified: Mon, 12 Oct 2020 17:33:00 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d2a750d0398afed62066488b9969e5363e7513d8e06aad3406a39391e32c42`  
		Last Modified: Mon, 12 Oct 2020 17:36:43 GMT  
		Size: 192.2 MB (192244841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5fade6d3cbf46df4c4b13ae73120928fc1bfe6b57f1ce64f7a67aa185a56b6`  
		Last Modified: Mon, 12 Oct 2020 17:33:01 GMT  
		Size: 3.5 MB (3512480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8de341009922726e4a352bf11fe1ec1275fd12ca71ecaf85a0edcfc4fad950`  
		Last Modified: Mon, 12 Oct 2020 17:33:00 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
