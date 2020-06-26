## `openjdk:16-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f8c61bb2c99349b109c859617f143bc00aa88ec123f8ef90da03a5e6eecf5a19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `openjdk:16-jdk-nanoserver-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull openjdk@sha256:cf54a547fbafea12078c9ae3d5f99bd8ce3f543c85b898ae9937a71912500c85
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.0 MB (295987937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e63d8d154558dbd030025c3aa9dcee4cdb1554cb1844d5787c24d66b498ac19`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Jun 2020 11:12:32 GMT
RUN Apply image 1809-amd64
# Tue, 09 Jun 2020 22:42:44 GMT
SHELL [cmd /s /c]
# Thu, 18 Jun 2020 21:20:54 GMT
ENV JAVA_HOME=C:\openjdk-16
# Thu, 18 Jun 2020 21:20:55 GMT
USER ContainerAdministrator
# Thu, 18 Jun 2020 21:21:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Thu, 18 Jun 2020 21:21:11 GMT
USER ContainerUser
# Fri, 26 Jun 2020 19:59:41 GMT
ENV JAVA_VERSION=16-ea+3
# Fri, 26 Jun 2020 20:00:33 GMT
COPY dir:338331b38588858de20adca88db521cdd4254b6156362dd8047028d501f8e4f5 in C:\openjdk-16 
# Fri, 26 Jun 2020 20:00:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 26 Jun 2020 20:00:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7d6d47ff7dfb2aa4d4e819641b93ec971e8541978dff0ffc24c193babeb8c07`  
		Size: 101.0 MB (101043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b390ee94e41353252b153770fa99d748992b90bdaf9abf7c785d93be52ee02c`  
		Last Modified: Tue, 09 Jun 2020 23:19:14 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6735890902f0d30df68ef896ea73cd7d60bdd05747cff4957193c1e609fff89a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee48b3407ba988368d7894a7733194fa4aa014b7f58f2d8c7fcaef8e2671a28`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 876.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6045b891a8218b59a2fddf2b6cac14838a3415c9d2d3092bc26b5e034902d9a`  
		Last Modified: Thu, 18 Jun 2020 21:28:21 GMT  
		Size: 67.2 KB (67242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f442edf533cb5c66c3872015a3894f657674d730051b398dd331afcfe90617`  
		Last Modified: Thu, 18 Jun 2020 21:28:18 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc6b2abb2042717b596072ad5543d0c33bb2ffbc10918b4b872c8b2a73d504c`  
		Last Modified: Fri, 26 Jun 2020 20:13:36 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c7a78ab86cb5b277b186231d450e238783a5089e71aa251de5342aec770487`  
		Last Modified: Fri, 26 Jun 2020 20:13:58 GMT  
		Size: 191.4 MB (191388729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3876781de88b8fbe9217ccc6b78496be4f6e0b5fe95d00277d2569bab07074f`  
		Last Modified: Fri, 26 Jun 2020 20:13:37 GMT  
		Size: 3.5 MB (3483259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6a40d328ca77887f1b3a0094f81dd7bbd3998a154a8848921658642aa7e305`  
		Last Modified: Fri, 26 Jun 2020 20:13:37 GMT  
		Size: 935.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
