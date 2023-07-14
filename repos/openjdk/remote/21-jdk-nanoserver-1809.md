## `openjdk:21-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:78e967940ab322e0e8a1e9a758d2e586a0af8018fb451427508134362abd5ef5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `openjdk:21-jdk-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull openjdk@sha256:4371d2fd690e04b67ca2c15a9356ddb8cb775cf8e7af0a9632cef8d9b5ce146d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306299191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83e317d3ba216b73021272f51af85c170105f4d7b3a2ba223466feb60b71750`
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
# Fri, 14 Jul 2023 00:20:03 GMT
ENV JAVA_VERSION=21-ea+31
# Fri, 14 Jul 2023 00:20:16 GMT
COPY dir:ef7258deb9dfa8379fe0a094dd79f4ab69315b37b52f33055460c9c8e8a5416a in C:\openjdk-21 
# Fri, 14 Jul 2023 00:20:30 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 14 Jul 2023 00:20:30 GMT
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
	-	`sha256:c3a6ab96ce074699205e61fe4c96f2ab409a80d8e21a5db009848db7b893540f`  
		Last Modified: Fri, 14 Jul 2023 00:24:58 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a19e71d02835bf9e130f267cc6ab2dc6edc90b7fc46fa4a619d1bdf7b5c2cc`  
		Last Modified: Fri, 14 Jul 2023 00:25:18 GMT  
		Size: 198.0 MB (197992193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670d5a6b18a4f3e4864bfadc0787a6e7785ebaa2530d5148fba85d9d6c06d248`  
		Last Modified: Fri, 14 Jul 2023 00:24:59 GMT  
		Size: 3.8 MB (3824188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5708f92c424d21b1b478a0ba22e8fcc6011e5470b8b1d07a67bfc9c70d7599`  
		Last Modified: Fri, 14 Jul 2023 00:24:58 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
