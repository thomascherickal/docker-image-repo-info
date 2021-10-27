## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:1ca745274002ff699149c872d26d6f46b6cf6a7ff3fcac6c580f7027bb0e3fbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull eclipse-temurin@sha256:37467559aad9eb459dd5cfe5063e073263aa997740e9f8e84085eeb552373aee
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294756179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc4f470b2b85fd55b8cb1f8542e6a8dd75ae97bb70fbe1ba6487076a693bac7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Tue, 26 Oct 2021 22:20:29 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Tue, 26 Oct 2021 22:20:29 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 26 Oct 2021 22:20:30 GMT
USER ContainerAdministrator
# Tue, 26 Oct 2021 22:20:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 26 Oct 2021 22:20:49 GMT
USER ContainerUser
# Tue, 26 Oct 2021 22:21:07 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Tue, 26 Oct 2021 22:21:28 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 26 Oct 2021 22:21:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bf1d9a4ed65dc7c2d297d6accf2237e8d3c392264abe115ab738f7512fb675`  
		Last Modified: Wed, 27 Oct 2021 00:28:30 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9ef8bb608957f2fa7a69ec5d555c99c76274b51e4a845469299710efbdf220`  
		Last Modified: Wed, 27 Oct 2021 00:28:30 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3260f5c3d01a05e2e0dbeb33f59ce0545312759c50bdd0cf6976915ce9e3262`  
		Last Modified: Wed, 27 Oct 2021 00:28:30 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17e2ad1c0a4e9019931b781569d9c7ed7587c0235de93c303788d0c9f51537a`  
		Last Modified: Wed, 27 Oct 2021 00:28:28 GMT  
		Size: 70.0 KB (70026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fde5701368c93a648331a822d4f92e37b8a08a1c4f1d4eabc9a1dfca7593da`  
		Last Modified: Wed, 27 Oct 2021 00:28:28 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80533950a5cc254337f1b308b4e01c489959724b243e1aa90e71d81e619c6fc7`  
		Last Modified: Wed, 27 Oct 2021 00:31:49 GMT  
		Size: 191.9 MB (191927150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290d744e8d185b1e0042d3b62cac237d750b4c30d0fbc86982f138a1e7818b78`  
		Last Modified: Wed, 27 Oct 2021 00:28:28 GMT  
		Size: 90.8 KB (90819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfc3032590554c1a72ecf8fd01f7a485b9741c038207576cca063c4b4ed4932`  
		Last Modified: Wed, 27 Oct 2021 00:28:28 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
