## `eclipse-temurin:20-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:080dc46f33825b44a77f209698809bdb42961e09a14d5f9fae09b3e6bbdc2736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:be8a1b3fb5a0fdadc06a72c3f0edd77aa6eaeadc44e8b1312ac57b77c14cdf49
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.5 MB (315452100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8c1bf7a4d83cefa7c63b7c42bd3662d652835d0bae62fe089bb29348e33356`
-	Default Command: `["jshell"]`
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
# Sat, 24 Jun 2023 01:12:52 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Sat, 24 Jun 2023 01:13:06 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 01:13:06 GMT
CMD ["jshell"]
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
	-	`sha256:d2ffde0d4e9027f0f34cf377cd4bca175ad25b9053ed604c31fee5567f6012f0`  
		Last Modified: Sat, 24 Jun 2023 01:37:06 GMT  
		Size: 195.3 MB (195274257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d500896d81a3623698b7649ef014dbdcea7500ff6a0b75409dc093dd159e6cea`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 62.0 KB (61954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d9ea34a1109200d8fb426c9c1ebbb74e71af13e10eeced69b3e7911142aeab`  
		Last Modified: Sat, 24 Jun 2023 01:36:45 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:20-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:52f1fa33ea89c9d0f6a57c32968bca651df30e1836cf6a51e7948f71470dd40e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303534724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058f63e88c1f6fe71610cbd2591ff8fa7565b145776508923188f92c2570fa8b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:04:02 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Sat, 24 Jun 2023 01:04:03 GMT
ENV JAVA_HOME=C:\openjdk-20
# Sat, 24 Jun 2023 01:04:04 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:04:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:04:14 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:04:29 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Sat, 24 Jun 2023 01:04:43 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 01:04:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09087aac643f57e5e24f95fe0a1c8519d0f93dfcf4500263516c0f3874290109`  
		Last Modified: Fri, 23 Jun 2023 02:23:11 GMT  
		Size: 104.4 MB (104400893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09be2e47b3dff420361e93d34eaadedcfd9549c9be5bd77936370792babf874`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f867d2c4f284f34f17dbc421aadc9e0fbec404d33de133b85670db5211e77528`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9299bed8971d729fd6ea364dd0fdea58af4cbed817932cdeadb0e2ce5280817f`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef55d7fc9b89fa790f54f2685e2644e68328f51c1bc1df43d652db4d15b32df`  
		Last Modified: Sat, 24 Jun 2023 01:32:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bae46e058dfc9dbf46033443d916af0a2155c758187110e18f5da39d047ef69`  
		Last Modified: Sat, 24 Jun 2023 01:32:52 GMT  
		Size: 69.5 KB (69460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5713507914a5a9e5750810b925cdffc1f0cb3a926b162f73e1360e13b4c7c1`  
		Last Modified: Sat, 24 Jun 2023 01:32:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe80f714c2a91038b32cd1e4dff02237ea5af0612834c62077b91165846179`  
		Last Modified: Sat, 24 Jun 2023 01:33:12 GMT  
		Size: 195.3 MB (195275307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ce68bb8b80a1270ea0d6e4d45f2dc2a45615f4fc52ccd73f9160eec99a28bc`  
		Last Modified: Sat, 24 Jun 2023 01:32:53 GMT  
		Size: 3.8 MB (3782037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8942927115a41d361e6c7172254481cb3bf21d5cfe20c86daa0845ebc75533c9`  
		Last Modified: Sat, 24 Jun 2023 01:32:52 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
