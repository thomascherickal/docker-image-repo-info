## `eclipse-temurin:18-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:471000a54bdff5f0664d569c1ad40dcba7e8cf7b8718a7445487ccd029785db9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:91cf8a7ef8ffc9423491d70711e0e8fb0bb2dda03f1ee18c0e6914842f09e2d1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304083864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51a79e2ac4d822e47f31db55e12909648e2726b6bf97bd23fb62941cd3f6f1d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 15:51:12 GMT
ENV JAVA_VERSION=jdk-18+36
# Wed, 13 Apr 2022 15:51:13 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 13 Apr 2022 15:51:13 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 15:51:20 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Apr 2022 15:51:21 GMT
USER ContainerUser
# Wed, 13 Apr 2022 15:51:35 GMT
COPY dir:2e742036aad301ef262998624b1ad05a0be865b4697e1fe99b4c522724f72462 in C:\openjdk-18 
# Wed, 13 Apr 2022 15:51:45 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Apr 2022 15:51:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5ee98801bdad72bc36678d072c89f7dd482fee29086c1d9c8ad6ff0cb5afa385`  
		Size: 117.6 MB (117579416 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:924a7c42e559a85c0bc74dbb028ddeee43fe67b0f59c81c60cbda0082e0e3ae5`  
		Last Modified: Wed, 13 Apr 2022 16:38:31 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c330e6984f1edaf84bd1fad30f7edeb83989e64e2390e37da7a4e0add0a755ca`  
		Last Modified: Wed, 13 Apr 2022 16:48:55 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d96746fb4c7ad3b364c239486f4e18fb5fd9be96b4f0a49c0b38a0422a63d7`  
		Last Modified: Wed, 13 Apr 2022 16:48:55 GMT  
		Size: 1.0 KB (1015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6192a80065952183007b6252a10d7aae670159ff6f31584f49ecf2cc29d5e181`  
		Last Modified: Wed, 13 Apr 2022 16:48:55 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074eb8e0ad7fbe2f056ccb47a56cd4631e2f2150909aba84f6f7e910e27e1d0b`  
		Last Modified: Wed, 13 Apr 2022 16:48:53 GMT  
		Size: 85.0 KB (85006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e633beabcd33a679fdcbcca0fd594331da035f4967f19bebb3eb735a7753772`  
		Last Modified: Wed, 13 Apr 2022 16:48:53 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d62b0dc301e19feeb5237cb819c12f715379a2f7d75c88288444815972ce6a`  
		Last Modified: Wed, 13 Apr 2022 16:52:06 GMT  
		Size: 186.4 MB (186350006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747083f79859c264bf4ee8437ab0e445bc6365159bdd151acdbeb419b403e60c`  
		Last Modified: Wed, 13 Apr 2022 16:48:53 GMT  
		Size: 63.1 KB (63080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf1206378e6f488729bc837dc49728a211497567de2b07a47b04f1c5bc0435f`  
		Last Modified: Wed, 13 Apr 2022 16:48:53 GMT  
		Size: 1.1 KB (1091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
