## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:15439e65429489de5c730679b9766f198c9b12326b519a6339e64ac2498ba36c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.587; amd64

```console
$ docker pull eclipse-temurin@sha256:c4ce58b136edef6147adea31c158272e06b7e29e1e4bbaae7b13d5bff28c78d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160742139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bead6f8d9dc9a33df47c3df139e54907aad27722c6e6abd141edd07a33efbe2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 04:50:34 GMT
RUN Apply image ltsc2022-amd64
# Tue, 08 Mar 2022 22:26:00 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:29:10 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:29:10 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 08 Mar 2022 22:29:11 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:29:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:29:23 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:30:19 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Tue, 08 Mar 2022 22:30:38 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:dad81795ce109a7e20ebf80ad31925797ed97f9ba2a559f13f96ce3be5ea712b`  
		Size: 117.5 MB (117485491 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ad17ae3a2fc5cdf554f0d828bd6d04e79f37ae3dd800a44c8a3a1892a57b75c3`  
		Last Modified: Tue, 08 Mar 2022 22:57:38 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a2d191ed154acbc5f87c0c16303ef84a425ae3b20ff0ef131d9d1f6ea1e0e9`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ef17868c695af7053447548c30b3befe6c902692291edd2706a6275a89631c`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8749dcdd44bfcf8927ece700e5ec010daad5c3daff63f5f9e993beba36fd11`  
		Last Modified: Tue, 08 Mar 2022 23:03:22 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc3a78d8d11295a20622c3299b08f453bf1417b8cfca0f7d3f4a12ee4b482fe`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 85.2 KB (85158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c5f95c2833f07d793777fbd4d6bcde63ff4fc108458e4531b21c3880b4fd2e`  
		Last Modified: Tue, 08 Mar 2022 23:03:20 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d7f473d1ae532f04d4cb735fe3f671707dd9777bdc152b17af671cfed9d5`  
		Last Modified: Tue, 08 Mar 2022 23:08:00 GMT  
		Size: 43.1 MB (43103923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da68ce9834f5da7a220855a03a0f9c413d6bbb30d44bf085f811d64466eb3942`  
		Last Modified: Tue, 08 Mar 2022 23:07:10 GMT  
		Size: 61.7 KB (61747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:ad37c1578b294ae0de93d8d8c95a3988bd90bfaeca528b88ed9536e0a8ae845a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.3 MB (149276962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e059022402ca0d44ff6530bd34d9a5c92a5346940ec9b6db34583b7e248a6c8f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 21:56:20 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 08 Mar 2022 22:20:40 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:20:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:20:54 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:25:34 GMT
COPY dir:7a64f3064f2760e9a3a0ea5871812392dd639be8dd87901cbb720c404830d2a7 in C:\openjdk-17 
# Tue, 08 Mar 2022 22:25:52 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e0065cd23a657c8f30ae5af121fd18451d2307835a1124ea57c80683eda26c94`  
		Last Modified: Tue, 08 Mar 2022 22:37:21 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e28e0120ae71480ac4b5292e1011f3e9a68e7648b992c086019524244ffc7f1`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d91688edda3231dbafc3286e5ecd7bcc1653c6a0e16cc01372b62928a409ef`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2195699d328d0527e400e78f2794d1150c371b24ac84f8bf12bba4aa47e9c2`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b8d01d40707a79981646b757c4bb673b5163d48f0f7e69f846dc526b2f5236`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 72.2 KB (72220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759cdd0f2650d033acdd0769c7ca2cf4ab535325556e99d303605abfbcbaccb0`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6712357b9729becd822b87483e767eb39301f51f44a5b550551dc1b0b2d04a5a`  
		Last Modified: Tue, 08 Mar 2022 22:57:26 GMT  
		Size: 43.1 MB (43111671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12c3ac61f7e11bec955fc793072cdd2d1b05c809cd8e5dd47f731f59d1b0d0a`  
		Last Modified: Tue, 08 Mar 2022 22:57:18 GMT  
		Size: 3.0 MB (3032812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
