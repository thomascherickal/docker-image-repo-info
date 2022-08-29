## `eclipse-temurin:18-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:49d108c510085fd15237127bafb4352c6945873f17b2e706d69c1cb5b7c622b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:18-jdk-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:7f2d8d91921acf44c6465b4427c42158ecd22295d032ef0fd6b03a03d55193b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.4 MB (293401056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a37aa6506efbde9820c8bbf49b1780d2f94510820db0f80fcb6a058879bc5af1`
-	Default Command: `["jshell"]`
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
# Mon, 29 Aug 2022 18:24:16 GMT
COPY dir:ae9d728ada666b27b908f8727aedf35273804bd829b96771abae3f99230f2142 in C:\openjdk-18 
# Mon, 29 Aug 2022 18:24:37 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Mon, 29 Aug 2022 18:24:39 GMT
CMD ["jshell"]
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
	-	`sha256:1bb951e66d1028712608596c4dba0123b6449ef788c4d7451a81eb299be02421`  
		Last Modified: Mon, 29 Aug 2022 18:36:09 GMT  
		Size: 186.6 MB (186551569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e3c5ee49f9a5e35eb53ee4d9cfd17851da73597a9c19ea23c4ead16fbc4c83`  
		Last Modified: Mon, 29 Aug 2022 18:35:52 GMT  
		Size: 3.6 MB (3567581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f1eca4649f841c1fa5c3327f2c41fd0a98c5aafb6dda3581a005b0ca988de8`  
		Last Modified: Mon, 29 Aug 2022 18:35:51 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
