## `openjdk:22-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:ec398d2e9d3ee6a381174cc828febf9e2f55a94925a5de1989d0e5a82a084d36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `openjdk:22-ea-jdk-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull openjdk@sha256:dca27c06f688d6954ea235fb8c534eb3cb2adc37d76361fd9f729233a02a6e8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (307041272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e62b793cdecfb6372372b7c7a5c18b160ebadb023308bedc752a830ddf40a821`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 03:06:42 GMT
ENV JAVA_HOME=C:\openjdk-22
# Sat, 24 Jun 2023 03:06:43 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 03:06:52 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 24 Jun 2023 03:06:52 GMT
USER ContainerUser
# Tue, 04 Jul 2023 01:43:13 GMT
ENV JAVA_VERSION=22-ea+4
# Tue, 04 Jul 2023 01:43:27 GMT
COPY dir:ab4b1ef2bbdd8e47a38b60e0ca3e198ccba29459d0292a694ed96d7b2ad10307 in C:\openjdk-22 
# Tue, 04 Jul 2023 01:43:40 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Tue, 04 Jul 2023 01:43:41 GMT
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
	-	`sha256:a0720397410cf27e11864dcfc2c9afadd7f7b2969f2bf4a2fd452cc3c6fdb541`  
		Last Modified: Sat, 24 Jun 2023 03:13:44 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2871b71eb8c2564d7544ebac7d7abbfc1ddd2570586a73f216323cab124eedc6`  
		Last Modified: Sat, 24 Jun 2023 03:13:44 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3912e3db7b6050feb04d0a6219277fd3a5cfb6649ccd27fe845538d11da2ec50`  
		Last Modified: Sat, 24 Jun 2023 03:13:44 GMT  
		Size: 68.8 KB (68757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57de6a9e2121836773f8d9f7079a0c6aab28ae6275690ecdee66946d9a774c6e`  
		Last Modified: Sat, 24 Jun 2023 03:13:42 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b491ce8f533b8addf4d77b8978db0b38ee509347e9a50585b76cdd5021ce8408`  
		Last Modified: Tue, 04 Jul 2023 01:48:37 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f7aa05059a29be6d20570d525608087d84c966da6d9415251f5b8afefdda2`  
		Last Modified: Tue, 04 Jul 2023 01:48:55 GMT  
		Size: 198.8 MB (198760713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b16055d9ea29903d8def5eea94104a9ac44ecec41633cadf1c0c1569593dfd`  
		Last Modified: Tue, 04 Jul 2023 01:48:38 GMT  
		Size: 3.8 MB (3804268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf849b696b8495ef3c30f9ba890971929252c9dc1a495be24cb74c3deeb8661`  
		Last Modified: Tue, 04 Jul 2023 01:48:36 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
