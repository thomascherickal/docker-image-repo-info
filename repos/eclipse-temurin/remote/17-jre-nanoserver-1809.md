## `eclipse-temurin:17-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:0dea951cf5d9d93bec07107141314e6e25751a0ac4ee2533a5f88fbf6f5281d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `eclipse-temurin:17-jre-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull eclipse-temurin@sha256:f4af9034b29d244117a3cd13c68c6a4ef337f643a714488b4d93077bf4755b95
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153137618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1185a18d68fc6c7df71ff002af771e8282279130ec245675e7c9af05cc70e724`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 15:20:49 GMT
SHELL [cmd /s /c]
# Mon, 07 Nov 2022 20:22:11 GMT
ENV JAVA_VERSION=jdk-17.0.5+8
# Mon, 07 Nov 2022 20:22:12 GMT
ENV JAVA_HOME=C:\openjdk-17
# Mon, 07 Nov 2022 20:22:13 GMT
USER ContainerAdministrator
# Mon, 07 Nov 2022 20:22:30 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 07 Nov 2022 20:22:31 GMT
USER ContainerUser
# Mon, 07 Nov 2022 20:27:54 GMT
COPY dir:20852dc87397947f41c5a6f7f30dc526aa127dbd27640e91343bc06b34d57a7f in C:\openjdk-17 
# Mon, 07 Nov 2022 20:28:09 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:ce29f4214f0fb0200b149c387d5e94ee47d5705e9bc7b884331390782282065f`  
		Last Modified: Thu, 27 Oct 2022 21:23:38 GMT  
		Size: 106.8 MB (106773776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a667d76c19fca171390d60fb90c40e16c777050e943a7fe17ad7686841f0f`  
		Last Modified: Wed, 12 Oct 2022 16:02:59 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574dc6cab5ebbd83429c51923e2ee334f317a0fa826a2e1e14fc2618052cf0d3`  
		Last Modified: Mon, 07 Nov 2022 20:35:45 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2726c1ef9a3e7bc42a0b77b459daa587d835f6fa0e6f75e7d123b5339237078a`  
		Last Modified: Mon, 07 Nov 2022 20:35:45 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793398beebfebf3a616e819b31f87bf1205ad081ddadbca43c8e59dc4ee29825`  
		Last Modified: Mon, 07 Nov 2022 20:35:45 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb349cdcba1e22a1177f86070953eb6a3dc64e1a937ca68fb067670a44bb409`  
		Last Modified: Mon, 07 Nov 2022 20:35:42 GMT  
		Size: 70.4 KB (70390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ac841c4b6b67338e81c8fb40d3128d82dd00d03341ae940a6f8bf1ccca87d3`  
		Last Modified: Mon, 07 Nov 2022 20:35:41 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f1e40ecd5ae576a5b977f3a19f253a7ed29076e7f2b0e200797a6a6029864f`  
		Last Modified: Mon, 07 Nov 2022 20:37:15 GMT  
		Size: 43.3 MB (43283686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c377b4ca7c2b66e3d10e1a42840787614430ca1a698505efe1a93aef074795a9`  
		Last Modified: Mon, 07 Nov 2022 20:37:05 GMT  
		Size: 3.0 MB (3004022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
