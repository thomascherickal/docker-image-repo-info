## `eclipse-temurin:8-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:8a4a6802b0550c5e1472461efce57b2f3b55aa45d581ac662334b60f7f117750
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8-nanoserver` - windows version 10.0.20348.887; amd64

```console
$ docker pull eclipse-temurin@sha256:ab4cf65c380a478baedc31f1ef10e4bfce01e71b635817b5a79f91b3bcb61381
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218710837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ecbff83ea28867efa129a69cf315409c66d37dda905555d242ae0539d00405`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 16:28:17 GMT
SHELL [cmd /s /c]
# Thu, 11 Aug 2022 19:27:02 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:27:03 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 11 Aug 2022 19:27:03 GMT
USER ContainerAdministrator
# Thu, 11 Aug 2022 19:27:17 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 11 Aug 2022 19:27:18 GMT
USER ContainerUser
# Thu, 11 Aug 2022 19:27:28 GMT
COPY dir:3f2d3aa63ba7a56176deaae1ba1b26dbdbe105074828954c77b0da527aacd6d7 in C:\openjdk-8 
# Thu, 11 Aug 2022 19:27:46 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f1e06146ab0490d235fe89786637467a4b71853ee428e8740ea6efbc536c47c`  
		Last Modified: Wed, 10 Aug 2022 16:48:40 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770dc366b2a629dc8c50641df646370966b4a3b3af562ea794b426e47acf9c31`  
		Last Modified: Thu, 11 Aug 2022 19:33:43 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b30283938410a8d67cf093632a7d78906fb7b27cfea2ff00306bdc483cd6c6a`  
		Last Modified: Thu, 11 Aug 2022 19:33:43 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb46b60d96d227e29a4c5423868410757fca4a805b6f1580031c016ce5aced9`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2900ae6f8b3a3c35c67bab56131b7dd5a1e658998d1a2002244f6783d06019d`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 84.4 KB (84440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54070f1ff08a7ab0078fc469730bb289ce25ea935871b8c6d4447f590ba639e2`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523f8d7b38db71243e121938cb6f33d7520bf0b80f4d61c2fb5055b8fc398da9`  
		Last Modified: Thu, 11 Aug 2022 19:33:52 GMT  
		Size: 100.5 MB (100469425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b258123d28cc3c8a7f57c9ef7629b223faeeacc72795ef2cf1cdfd378ea4fee3`  
		Last Modified: Thu, 11 Aug 2022 19:33:41 GMT  
		Size: 62.8 KB (62759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull eclipse-temurin@sha256:d307bb8d4a54ebc86052cb8e4bc18ede4a53d2308b370d4e41f3bc0a03bb5aa2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203844657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791355155584c5871eba892cc84d5cb3f3eaf91cf31df7b5cfd053b6265dba05`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Thu, 11 Aug 2022 19:20:23 GMT
ENV JAVA_VERSION=jdk8u345-b01
# Thu, 11 Aug 2022 19:20:23 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 11 Aug 2022 19:20:24 GMT
USER ContainerAdministrator
# Thu, 11 Aug 2022 19:20:38 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Thu, 11 Aug 2022 19:20:38 GMT
USER ContainerUser
# Thu, 11 Aug 2022 19:20:49 GMT
COPY dir:3f2d3aa63ba7a56176deaae1ba1b26dbdbe105074828954c77b0da527aacd6d7 in C:\openjdk-8 
# Thu, 11 Aug 2022 19:21:04 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fd3474e767c89d4884899365be25930e54c53f51a074e69cc02802725ae6d5`  
		Last Modified: Thu, 11 Aug 2022 19:32:12 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7647596c60b4a6ad1f5ca775c5fd3f55ff77837639afff14c18ba7835f2308`  
		Last Modified: Thu, 11 Aug 2022 19:32:12 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41014c3c1e1598b5823b5cfb25e91bc92911535419ec9cfacd6999e6d75c287d`  
		Last Modified: Thu, 11 Aug 2022 19:32:09 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a389d300354d5cae214dd02ea0250b75df400fc6dbdfe3a86010e1f0d8c3adbb`  
		Last Modified: Thu, 11 Aug 2022 19:32:10 GMT  
		Size: 70.4 KB (70417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc85db5fff9936a95dff8f64641330a3b012a5f63626ce212e03a832c9e2aed8`  
		Last Modified: Thu, 11 Aug 2022 19:32:10 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a787b21f44fd5281051f0fea6151f221a0e7fa19c6af6581e33b2b818b3716bb`  
		Last Modified: Thu, 11 Aug 2022 19:32:22 GMT  
		Size: 100.5 MB (100482248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda13d666f201160f3797318a706975f1fd764f1ef58cd667d81c534db79e54c`  
		Last Modified: Thu, 11 Aug 2022 19:32:09 GMT  
		Size: 82.0 KB (81980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
