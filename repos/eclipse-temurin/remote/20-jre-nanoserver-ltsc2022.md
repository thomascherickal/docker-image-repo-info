## `eclipse-temurin:20-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:2f839b5585912352900e7cbdcb281b8153061d4b214a41d3043180139967e0c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:20-jre-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:7fc3c537564eff3cea58d1902da95ee4333901e93020fd5897b51bd07158d044
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165933020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4561adf66f3709c59ee8b1bbbf27a4a4329dcd708b65de74054c5d8cc452ac56`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:12:24 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:12:25 GMT
ENV JAVA_HOME=C:\openjdk-20
# Sat, 24 Jun 2023 01:12:26 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:12:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:12:36 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:13:24 GMT
COPY dir:db4e97c4fd2cfe51abaeb1dfe2097f2044faeb2be3c3c04299b9c20e07c77033 in C:\openjdk-20 
# Sat, 24 Jun 2023 01:13:38 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81a88fd1e4270664dec2ec13169bd88eaa6b8b019c0fb48e06635378a709617`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c800fc714f89a75e5414a4597fac693e9d62be65fbd8c222f44cda41f44bc3`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfabed7da3438545b6544d6e2199c88812bd45e313099b56799677cbdc6662d`  
		Last Modified: Sat, 24 Jun 2023 01:36:47 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc81fe92368b73ce26b0fdba745b718c2f43c9c41458f9e7e0a7322ee849e7e0`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 80.7 KB (80715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f4a0aeb9583372b005ddce4994d5e31d4073d82f3d3fc4dd8d7efa1238aef9`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d9caedc8c1342cae7cfc87ab575e5b7cc64b8f1a943d0e475229e3990a6e7d`  
		Last Modified: Sat, 24 Jun 2023 01:37:26 GMT  
		Size: 45.8 MB (45757473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d443337d9ac727b245f3d032f42e5578d129d06e963b5b75dfccb9bde98f43d2`  
		Last Modified: Sat, 24 Jun 2023 01:37:17 GMT  
		Size: 60.8 KB (60794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
