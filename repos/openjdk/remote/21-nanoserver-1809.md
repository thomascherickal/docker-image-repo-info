## `openjdk:21-nanoserver-1809`

```console
$ docker pull openjdk@sha256:a78eb37cac2ed9b3253920d6fb02c0c5730029d2b1ab17a47173758fe513864f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `openjdk:21-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull openjdk@sha256:746067cd9458da2e4ca44c455c090cfb1748575c30c23d31df51e715d1f9deb2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306332433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37ce9bc4a4f968767617906bf9a2cf92e05c758d59bba7246f79b50134241ee0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Fri, 14 Jul 2023 00:19:53 GMT
ENV JAVA_HOME=C:\openjdk-21
# Fri, 14 Jul 2023 00:19:53 GMT
USER ContainerAdministrator
# Fri, 14 Jul 2023 00:20:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Fri, 14 Jul 2023 00:20:02 GMT
USER ContainerUser
# Thu, 03 Aug 2023 01:03:48 GMT
ENV JAVA_VERSION=21-ea+33
# Thu, 03 Aug 2023 01:04:06 GMT
COPY dir:d718de3dbf998b3e9b9d1efc9eb1d59fb69fab172cdc2206708bcca7798fdeb0 in C:\openjdk-21 
# Thu, 03 Aug 2023 01:04:17 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 03 Aug 2023 01:04:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289ea5fc8a7f31b38120d64f4fc304a5e09ac629f99bc9b5e92a4349bcf143bf`  
		Last Modified: Fri, 14 Jul 2023 00:25:00 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66b7bdcadf86bdda397cf414ae45f974a40e697d5002156e00e7cd59e946cbc`  
		Last Modified: Fri, 14 Jul 2023 00:25:00 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d929e2c9bf4cff0381fd000609dc5a373e8d51ceaca78fe43f609176c7d62d78`  
		Last Modified: Fri, 14 Jul 2023 00:25:00 GMT  
		Size: 67.7 KB (67668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ab158d7279412c8630521a444777102ad52479439f793e296ac44ef396e701`  
		Last Modified: Fri, 14 Jul 2023 00:24:58 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff66230591b7fddf8965794fc3e177177269e255fb8307f6191362f5c0bbdee`  
		Last Modified: Thu, 03 Aug 2023 01:43:11 GMT  
		Size: 1.1 KB (1073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9ae0e9ba8377960070c5317d3d8dfdf63c95a34f2f4fc373c92f8cc9a7cf26`  
		Last Modified: Thu, 03 Aug 2023 01:43:32 GMT  
		Size: 198.0 MB (198036025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c777fff341a93d02079934fc4962a782d05a7b226b1807cbd48b36dc345ea8`  
		Last Modified: Thu, 03 Aug 2023 01:43:13 GMT  
		Size: 3.8 MB (3813769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406b7e7a6efd5288d43276da16e1e3a01273de6d170a51343cbf036c115421d1`  
		Last Modified: Thu, 03 Aug 2023 01:43:12 GMT  
		Size: 1.1 KB (1055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
