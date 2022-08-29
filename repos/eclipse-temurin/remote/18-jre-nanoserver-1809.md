## `eclipse-temurin:18-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:5273547b1e77b0fe69e9cc8194d38a9dd03718a912762b2e2a3376566f8bd6de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:18-jre-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:143f3f0cca5efd91a1fbeb7f5f4b612cd94574bf686c2a1b2ddf2dc931788139
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149362454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f98d1f1a55e13d40b8a96d383b1f9b06e71963c9d4ec0aba3258d3ba824773`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Mon, 29 Aug 2022 18:23:38 GMT
ENV JAVA_VERSION=jdk-18.0.2.1+1
# Mon, 29 Aug 2022 18:23:40 GMT
ENV JAVA_HOME=C:\openjdk-18
# Mon, 29 Aug 2022 18:23:42 GMT
USER ContainerAdministrator
# Mon, 29 Aug 2022 18:23:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Mon, 29 Aug 2022 18:23:59 GMT
USER ContainerUser
# Mon, 29 Aug 2022 18:28:41 GMT
COPY dir:0f122a29933687aee1aeb1ed0bbcab77514458b9f4eb8e7fa2df7c081ea3d7bd in C:\openjdk-18 
# Mon, 29 Aug 2022 18:28:56 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079c8019b8d860add7e469efe084e361401eccb80eea879d6cbe4aaf0739d422`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff09b635a581659c5e7a0c8e3757bf70e464f2ccadd4cfca1d216e1f9a62bc8`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c09109e3ba671de263b5e0254bf16697599a7f4cff277eac6b17b536d8da26`  
		Last Modified: Mon, 29 Aug 2022 18:35:54 GMT  
		Size: 1.1 KB (1117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d5855590b900da119bf781ec14b2275d8ad785c2c621f2ace60dac79740a34`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 70.8 KB (70812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9b924fc322681a5fbbcc5b5c5f0d6108d37616bacd0d613e1e9fe685e41c52`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01601f091dc7483a14152d559c249e6c83432f035e7d97eea906253b04c7a282`  
		Last Modified: Mon, 29 Aug 2022 18:37:12 GMT  
		Size: 43.1 MB (43138172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9d68ced9dabd223d70d9bc2834643947ec4e398feefe6e2e7e24f44bea4ef4`  
		Last Modified: Mon, 29 Aug 2022 18:37:05 GMT  
		Size: 2.9 MB (2943548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
