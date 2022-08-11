## `eclipse-temurin:8-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:2b73c8c3df6d06eda6d92965e57465390ec8d4e36da6b71c83991f9943645f27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `eclipse-temurin:8-nanoserver-1809` - windows version 10.0.17763.3287; amd64

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
