## `openjdk:11-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:30ae2c066888d207144b1f4c023f01ff99d6f7a385bcc3aa528ca45d876eb77c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:11-jdk-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:13b48918a5acb08cd66ca845f7427bd68a285cfdbf36500ead11d59eb00f2efd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.1 MB (294066730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e293b278c087f501ea573bd2de471ef937b0c1576f63ee66d4e80a86b470d87`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 05:18:44 GMT
SHELL [cmd /s /c]
# Sat, 18 Dec 2021 07:29:30 GMT
ENV JAVA_HOME=C:\openjdk-11
# Sat, 18 Dec 2021 07:29:31 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 07:29:41 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 18 Dec 2021 07:29:41 GMT
USER ContainerUser
# Sat, 18 Dec 2021 07:29:42 GMT
ENV JAVA_VERSION=11.0.13
# Sat, 18 Dec 2021 07:30:01 GMT
COPY dir:f01eefe625ed2bb6eb89bcf5026bd8d3026198beb85b7d142c1a8700b8e43668 in C:\openjdk-11 
# Sat, 18 Dec 2021 07:30:13 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 18 Dec 2021 07:30:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4c557aac927613dd487d7c04b01a8eeb8ad174693f61b14c8f4285f1db6afdd2`  
		Last Modified: Sat, 18 Dec 2021 06:13:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14eb2f2d801166146f971e21cbbda55a7c4f005fef0ba1917e7930633516c8b9`  
		Last Modified: Sat, 18 Dec 2021 11:28:34 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51cd69dcd8582a3fb898e722cc22d2c315c748a8887a2b8880c7d4c64aac1e`  
		Last Modified: Sat, 18 Dec 2021 11:28:34 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1f7180157caa0fabf1418326832bbab664411ad6150f42f0adcd08e1fb0a76`  
		Last Modified: Sat, 18 Dec 2021 11:28:34 GMT  
		Size: 70.1 KB (70095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2883ac8c3ef6efd73eb729691aaa9bda29a4456f54c8aae25c11eb3a46e7a03b`  
		Last Modified: Sat, 18 Dec 2021 11:28:31 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0edc3c53eab49c7c55987cd69281b43b90445d544facf0365d5013b27072fec`  
		Last Modified: Sat, 18 Dec 2021 11:28:31 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f702dee756c1e5df9dd73974504aafe1ff29dbd40b80866ac64ead28c3fe1c62`  
		Last Modified: Sat, 18 Dec 2021 11:28:52 GMT  
		Size: 191.0 MB (191003067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091ee65cbe4b00aeb555073a9ee7570b7648c09cd3be88f8098f941704bc217`  
		Last Modified: Sat, 18 Dec 2021 11:28:31 GMT  
		Size: 82.6 KB (82644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6290ba9fda96b6885880eacd0bb55a6ab626808b9105377f820c50108ec9e6`  
		Last Modified: Sat, 18 Dec 2021 11:28:31 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
