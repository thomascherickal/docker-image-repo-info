## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:312b18443236045eecc69120667c57433584c4e02e2ecd59bd3f53ef2a55904f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:c7d0feb2b81d12afa4560a1531073bd4f06305e0e5f52c79adbbec29dea97465
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142469483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6215c3b0461b9bd56ad901fddd3658e53a32839daa30b5a61f1524c39437f28c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 18 Dec 2021 07:34:15 GMT
COPY dir:63916d6bee2220e36f2a9872b4f6dbefd913ce14199f5f87aa18e7a5987717fa in C:\openjdk-11 
# Sat, 18 Dec 2021 07:34:28 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
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
	-	`sha256:fe047734f462044db307344f850170cec05cfc9c74a97ab4866f4a90362d0d1b`  
		Last Modified: Sat, 18 Dec 2021 11:31:29 GMT  
		Size: 39.4 MB (39407663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd58e72a847dfa1bb4bc1f7b8b3ccc79f714f36a66697725fe15f1beb6c1563`  
		Last Modified: Sat, 18 Dec 2021 11:31:21 GMT  
		Size: 82.0 KB (81969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
