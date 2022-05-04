## `eclipse-temurin:18-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:cb84bb7f9e362b3f5aa6d14846a50ab5e44d28d8840b30a06ccfb16e7b9d036e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `eclipse-temurin:18-nanoserver-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull eclipse-temurin@sha256:1f7a516e8b03927a83a941fb6bbd2cc753c84b23e3bd60c27b83318efa78d522
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304148706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e7b2bc3f82564a7c19ad5ec372c3c6f88b92969e587aa4c88e785b9fd6f5c6e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 03 Apr 2022 05:29:07 GMT
RUN Apply image ltsc2022-amd64
# Wed, 13 Apr 2022 15:47:59 GMT
SHELL [cmd /s /c]
# Wed, 04 May 2022 18:28:26 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:28:27 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 04 May 2022 18:28:28 GMT
USER ContainerAdministrator
# Wed, 04 May 2022 18:28:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 04 May 2022 18:28:35 GMT
USER ContainerUser
# Wed, 04 May 2022 18:28:50 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 04 May 2022 18:29:01 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 04 May 2022 18:29:02 GMT
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
	-	`sha256:089a88f54de05890eaab4cbd37399afff42f7c5a9f550a19ed7962758a221939`  
		Last Modified: Wed, 04 May 2022 18:36:11 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d16e4f5a8aeb16031deb5c6584de9e4305697e9e1a3d44c591d95879e7d09a`  
		Last Modified: Wed, 04 May 2022 18:36:11 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429f7366067083ae01419dd31e6e105cf84b82a5b7f91b812bc60cfb58c92a4c`  
		Last Modified: Wed, 04 May 2022 18:36:10 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b858cdf486d22d72c1a9c9ddd294e947fd16a4004d6428626dec088a50440f2`  
		Last Modified: Wed, 04 May 2022 18:36:09 GMT  
		Size: 82.2 KB (82245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee2117aee9f2bae1b8685e7023b8ada6f81a5ef6e467c3fe506e7fa016a97b7`  
		Last Modified: Wed, 04 May 2022 18:36:08 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940909417c2f57293b9bdfcd034d7321da0be8d1c4eb21b77a722d5d5fece832`  
		Last Modified: Wed, 04 May 2022 18:36:27 GMT  
		Size: 186.4 MB (186417012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28584ba6323aa2489c4b765bbb8dcbd65b8dbb1d2fbdf8eac587d9e1f50cf7c0`  
		Last Modified: Wed, 04 May 2022 18:36:08 GMT  
		Size: 63.2 KB (63242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2fb2955c31b3790b840a6212ca6516405da7402ad44f1c5451d21b4b43867`  
		Last Modified: Wed, 04 May 2022 18:36:08 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
