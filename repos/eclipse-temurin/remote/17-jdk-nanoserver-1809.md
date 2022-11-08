## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:936a855ab576e952084dc7107f50e9e218ee2228f52c0b35b3c58becaffc1c86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull eclipse-temurin@sha256:741a83c3b92e6f5ce1f9ddb87f7c69825fd49a23876189b39c38c7a6887b51c2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295925326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48fe0c798228f8b2d46d2d795d9cfd0e39ee509269de893eefc356577aa41ab7`
-	Default Command: `["jshell"]`
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
# Mon, 07 Nov 2022 20:22:49 GMT
COPY dir:a12ba5a18c812bc88dc6c1e12f0d0bdbacab70db88697cd6bad273d4570ac4fb in C:\openjdk-17 
# Mon, 07 Nov 2022 20:23:18 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 07 Nov 2022 20:23:19 GMT
CMD ["jshell"]
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
	-	`sha256:f827f825260c65af7b9a2ceb13a96ff8dd5c2fc70758be5312c08442231c19f3`  
		Last Modified: Mon, 07 Nov 2022 20:36:04 GMT  
		Size: 185.4 MB (185427997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c923a36bbc008fcfc5b62ecb08d1d3119991d8419c8ef07f554abe6416538944`  
		Last Modified: Mon, 07 Nov 2022 20:35:43 GMT  
		Size: 3.6 MB (3646243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5155809da6dae90aa0fe4b57dd4ff4b0473159b1423e0a9b935891bc97107dcb`  
		Last Modified: Mon, 07 Nov 2022 20:35:41 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
