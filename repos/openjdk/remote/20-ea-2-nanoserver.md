## `openjdk:20-ea-2-nanoserver`

```console
$ docker pull openjdk@sha256:d31e36888cea3b052617dce10a7ce1661b3d0e5865b35859ab39b6aef5abe06e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `openjdk:20-ea-2-nanoserver` - windows version 10.0.17763.3046; amd64

```console
$ docker pull openjdk@sha256:d97e871ed1fcd30f4a418b087667c7f1e1f7ee2904851685aba616d04ff5011b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299164662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8baf76666b3def54bdef4e3e10888234cec54161ed994d55fbf3fe80097010e4`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 09 Jun 2022 19:20:11 GMT
RUN Apply image 10.0.17763.3046
# Wed, 15 Jun 2022 17:30:58 GMT
SHELL [cmd /s /c]
# Thu, 16 Jun 2022 01:19:36 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Jun 2022 01:19:37 GMT
USER ContainerAdministrator
# Thu, 16 Jun 2022 01:19:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 16 Jun 2022 01:19:50 GMT
USER ContainerUser
# Wed, 22 Jun 2022 00:47:03 GMT
ENV JAVA_VERSION=20-ea+2
# Wed, 22 Jun 2022 00:47:19 GMT
COPY dir:b58107e9577c2b6d3209c18ace56fc343e1e7684cd5113beeef965a5339d9547 in C:\openjdk-20 
# Wed, 22 Jun 2022 00:47:41 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 22 Jun 2022 00:47:42 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d555a7e4de4dd775379d5c43c1419374bff7908670dc7444be5e8e8f386f3d26`  
		Size: 103.2 MB (103153235 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:92b4c385cd5cbb12fb09cb31c12b5e5de38cf7b380c8681286caac242c06d3ed`  
		Last Modified: Wed, 15 Jun 2022 18:22:11 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda95a4aa1ce8b324ff84e1ccdf8befbe50e58a948d31b65618925e2842efada`  
		Last Modified: Thu, 16 Jun 2022 01:33:30 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f66084dce2c5c1fa8b13cd8edb172b48a4411ebf5466035c9c5fef517796cce`  
		Last Modified: Thu, 16 Jun 2022 01:33:30 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a225993ae008c14a2ad71f55edbcafc99d581fba5b2fd8297a2af9bd6fc2d`  
		Last Modified: Thu, 16 Jun 2022 01:33:30 GMT  
		Size: 71.2 KB (71215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1582199825c588de3fcfbec196a74a70813b8a78abaa2abbed131795de8f1d6`  
		Last Modified: Thu, 16 Jun 2022 01:33:27 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d2ebb203c0b13c4c0a328a7f741c40279c87e9af9e5d683445d5332f8cf6c7`  
		Last Modified: Wed, 22 Jun 2022 02:28:46 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5112eaadca8ab7fc1a0af4a83fea14d40565a7e1cf151d01dd8731f26286298`  
		Last Modified: Wed, 22 Jun 2022 02:32:07 GMT  
		Size: 192.2 MB (192203103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c627afacdd82ddd376f9ef358a48857e6ef96992861e5c3ceaa83293bab96b`  
		Last Modified: Wed, 22 Jun 2022 02:28:48 GMT  
		Size: 3.7 MB (3730152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e26d2bab55b3e3c78fe987d59e4cc37a64867a02dce0135f4a3b763cd923aec`  
		Last Modified: Wed, 22 Jun 2022 02:28:46 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
