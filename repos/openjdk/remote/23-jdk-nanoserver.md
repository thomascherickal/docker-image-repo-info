## `openjdk:23-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:6fad7f411b8053df4de5234a84450049f7bede9bd84c110654a47ebada673723
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `openjdk:23-jdk-nanoserver` - windows version 10.0.17763.5206; amd64

```console
$ docker pull openjdk@sha256:5d2a89324fcaae1f9e40e4e42f7eca782f877fe3df76b4cbb288e93bb6dd99f5
```

-	Docker Version: 24.0.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305827957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f76ace61e8c48e4b13798a4bd38d6a3c2f66c411342a71c8b53e4b64e864a99a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Sat, 16 Dec 2023 00:02:18 GMT
SHELL [cmd /s /c]
# Sat, 16 Dec 2023 00:02:21 GMT
ENV JAVA_HOME=C:\openjdk-23
# Sat, 16 Dec 2023 00:02:22 GMT
USER ContainerAdministrator
# Sat, 16 Dec 2023 00:02:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 16 Dec 2023 00:02:26 GMT
USER ContainerUser
# Sat, 16 Dec 2023 00:02:26 GMT
ENV JAVA_VERSION=23-ea+1
# Sat, 16 Dec 2023 00:02:34 GMT
COPY dir:91fce60f2d61fb668a105ab54f9d6be86b9555f36ebf342ed491e4034b82d84c in C:\openjdk-23 
# Sat, 16 Dec 2023 00:02:39 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 16 Dec 2023 00:02:40 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c669cc727e2e5b88bff9b788f3fcca8f9e194aa87ec8e71c0a5b91920bf3a482`  
		Last Modified: Sat, 16 Dec 2023 00:02:45 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202fa1e50ec84f82f07d97f0011ef6dbd34699476ba33c127044cf8bf67ec3ea`  
		Last Modified: Sat, 16 Dec 2023 00:02:44 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0f8bef19523ae9f30bbd075d0d13411cc090dfdff0606b0b75ce41950eda66`  
		Last Modified: Sat, 16 Dec 2023 00:02:44 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa66465a8fc2f5e81a5ca9004771d5719d85558fbf5a7367b541ccfdd938c685`  
		Last Modified: Sat, 16 Dec 2023 00:02:44 GMT  
		Size: 71.6 KB (71585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0692ae490c6c76ae41cda6efa5b68e25ddc217aba6e1140d943fb1ecfb967`  
		Last Modified: Sat, 16 Dec 2023 00:02:42 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00d136b42057078af6d24685dade98b74b811653ae7cbbe076cac6f0c7e0520`  
		Last Modified: Sat, 16 Dec 2023 00:02:43 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5c3c977defcb14a218620e692ad6fc1d42148c19acf197b917e465b26544b7`  
		Last Modified: Sat, 16 Dec 2023 00:02:54 GMT  
		Size: 197.4 MB (197383832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1eaf0b762bc24efcf7bc6aba584a310c7d741de74f44831088b63233f3282`  
		Last Modified: Sat, 16 Dec 2023 00:02:44 GMT  
		Size: 3.9 MB (3856252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68354d5ea9aa5665979964a015d9d9776b55a3e367b0b2fcd8abd2351c05d8e`  
		Last Modified: Sat, 16 Dec 2023 00:02:43 GMT  
		Size: 1.0 KB (1010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
