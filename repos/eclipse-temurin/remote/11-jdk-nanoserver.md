## `eclipse-temurin:11-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:5d48b16fd75455180dc27266e73ee9753e67468ad7041f3f6c8f4dd393fd482f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.288; amd64
	-	windows version 10.0.17763.2237; amd64

### `eclipse-temurin:11-jdk-nanoserver` - windows version 10.0.20348.288; amd64

```console
$ docker pull eclipse-temurin@sha256:33b0746b05bcd5aac0f3b80b67622cd6d9a669c084f5f66b3ad9628530a777e5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.0 MB (309013455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74a28afba8977cfc4e1a27ca78b81d4e4d99a13fd7af5aad9cd9d14e6d280431`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 11:15:04 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Oct 2021 19:02:30 GMT
SHELL [cmd /s /c]
# Tue, 26 Oct 2021 22:27:04 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Tue, 26 Oct 2021 22:27:05 GMT
ENV JAVA_HOME=C:\openjdk-11
# Tue, 26 Oct 2021 22:27:05 GMT
USER ContainerAdministrator
# Tue, 26 Oct 2021 22:27:26 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 26 Oct 2021 22:27:27 GMT
USER ContainerUser
# Tue, 26 Oct 2021 22:27:44 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Tue, 26 Oct 2021 22:28:05 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 26 Oct 2021 22:28:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:91284e7e8fd4bd7ebcfa98544a3e4f59639f38281225c81c34b6fe22e0dba4e5`  
		Size: 116.9 MB (116939483 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ba797e8f93823c3d71c52fcae413f3a33ca28ff2711c09ba5141432948f8298`  
		Last Modified: Wed, 13 Oct 2021 19:43:54 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5496de008b770ec467d4156c4492e726ea95aacc468ead67297672335d946c3d`  
		Last Modified: Wed, 27 Oct 2021 00:33:04 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966e7576b2e9bf1bda4b03bc28938ca36d1725bc17494b2c11d6670d064a2551`  
		Last Modified: Wed, 27 Oct 2021 00:33:04 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb6df87291b64e881c924fa31b55558489e0aef315ac3bea896b2a6526894c8`  
		Last Modified: Wed, 27 Oct 2021 00:33:03 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ca23fc1aca87db648be45d76f6226d6a81ca9b6cfcbdc090eb82647b04b378`  
		Last Modified: Wed, 27 Oct 2021 00:33:01 GMT  
		Size: 79.8 KB (79756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71abbdb585b9b63c845550e8557957f5341227a10b425691575a040558888733`  
		Last Modified: Wed, 27 Oct 2021 00:33:01 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4bc5d80531961fedc213cc96447adcbd6101dc18f4df014c67fc82320d10e9`  
		Last Modified: Wed, 27 Oct 2021 00:36:30 GMT  
		Size: 191.9 MB (191924220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e055131b4d000d9c059f62e2d8f9675e18d63dbee90163b6c7efab91b1fd1`  
		Last Modified: Wed, 27 Oct 2021 00:33:01 GMT  
		Size: 63.1 KB (63075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6f9ead72ca3a5e396225d6e918db16b6fb32273e42264afe03effd7d78544d`  
		Last Modified: Wed, 27 Oct 2021 00:33:01 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-nanoserver` - windows version 10.0.17763.2237; amd64

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
