## `eclipse-temurin:11-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:594fba21801f60fac7846550fcb23e55f398a0472df6a6c06381297999ec0cb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `eclipse-temurin:11-jdk-nanoserver` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:a3f1c6d477117366b184c7442a3b794e48375a984efba0bda06852a8192cda57
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.1 MB (310057872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed016f4c2f339f394c7e585a3f91649f2f742c06f17586627de0855c32d41cb5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:23:24 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 11 May 2022 15:23:24 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 May 2022 15:23:25 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:23:37 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:23:38 GMT
USER ContainerUser
# Wed, 11 May 2022 15:23:53 GMT
COPY dir:1583ce76f01a2d0a0742f7b70646c210ef8c619565a381c37e5a1156f6ec4636 in C:\openjdk-11 
# Wed, 11 May 2022 15:24:11 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:24:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5d189c2aec305bffe94fd2b3728517b2b2388f7c112834045a40c9dd163943`  
		Last Modified: Wed, 18 May 2022 13:45:19 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2573b8ff607047440c04273d12b721b1d86da7ab3c55fd8fabb56418ef14799d`  
		Last Modified: Wed, 18 May 2022 13:45:19 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5266fa1a5136e3b49c17ee4b66c6580b283f9ba9826ed12d53435dff0da365f6`  
		Last Modified: Wed, 18 May 2022 13:45:19 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da3bf4fa48c42b9405385f5aaa04f8d453fa22cfed35ae10073ab55fc39916d`  
		Last Modified: Wed, 18 May 2022 13:45:17 GMT  
		Size: 77.6 KB (77589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b892a3073093f69522e0f26ce522c4b2476ffe648e8e2cb205980887028b2c05`  
		Last Modified: Wed, 18 May 2022 13:45:17 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fe094ea48ae294d3545540108bc742a28f6893c0dc148f9a5d6874a35bd16d`  
		Last Modified: Wed, 18 May 2022 13:48:35 GMT  
		Size: 192.2 MB (192225580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732cdbab880343fbe7d8611ba3e7b444c76a41f572b20b6e986a5346954a1046`  
		Last Modified: Wed, 18 May 2022 13:45:17 GMT  
		Size: 60.8 KB (60793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a93123eed4acf3e8429eaf240b1ba3600e908ee9114cc049ec865857e6afad`  
		Last Modified: Wed, 18 May 2022 13:45:17 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jdk-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull eclipse-temurin@sha256:3d4fd2a402fed2c38adde42800bc526e0234ad292edf8f13fc86c8c446ce1616
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295491092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a92cae6eea5dae3d18fc2031a35c69fb818523d265372c715251fea660fc7e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 14:58:58 GMT
ENV JAVA_VERSION=jdk-11.0.15+10
# Wed, 11 May 2022 14:58:59 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 May 2022 14:58:59 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 14:59:09 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 14:59:10 GMT
USER ContainerUser
# Wed, 11 May 2022 14:59:24 GMT
COPY dir:1583ce76f01a2d0a0742f7b70646c210ef8c619565a381c37e5a1156f6ec4636 in C:\openjdk-11 
# Wed, 11 May 2022 14:59:39 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 14:59:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0368d8c7dd50aefc640bd0e9ec5c4ac0fbb965d3a6c6eea9e64941e2ea35be5`  
		Last Modified: Wed, 18 May 2022 13:06:36 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f24cf7e5731f61d079e3a2f190da5e1e4b8b6281fb04594c4b460868a6c44b4`  
		Last Modified: Wed, 18 May 2022 13:06:36 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f07638ea9d8eb9d00a4a5d7bad819130ef62cafb4e830806bc3284e5e32c51`  
		Last Modified: Wed, 18 May 2022 13:06:36 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2539ecf1e806d52a807ca84428fc8bc317f7318d5553f3f90bf69582c63168ab`  
		Last Modified: Wed, 18 May 2022 13:06:34 GMT  
		Size: 75.7 KB (75695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16f62ce98a0966a7a3106565055ad93b30f48519286387318fc054d1ac83b21`  
		Last Modified: Wed, 18 May 2022 13:06:34 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f464ad35de6c23341eafcc2ca99beeaeb6a4e8786958af2690e7a69844ed2b5a`  
		Last Modified: Wed, 18 May 2022 13:10:02 GMT  
		Size: 192.2 MB (192225346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46582cb5881e05922a58c3885b024e68c5cb2ae52be50162e975222d8099fbf`  
		Last Modified: Wed, 18 May 2022 13:06:34 GMT  
		Size: 49.2 KB (49239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245a0088dbe8c5626d10a6b8132bcf0df16095843b850fa7ba55114afbc6776e`  
		Last Modified: Wed, 18 May 2022 13:06:34 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
