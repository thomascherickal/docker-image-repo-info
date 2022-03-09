## `eclipse-temurin:17-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:9355b9e2b185b0e84606ce2175a9ede5c7c17acbdd358c6b6f52115af780bc69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `eclipse-temurin:17-jre-nanoserver-ltsc2022` - windows version 10.0.20348.587; amd64

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
