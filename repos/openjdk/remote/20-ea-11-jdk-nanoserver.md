## `openjdk:20-ea-11-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:2141da91fb448aa839352e55cf6a0e85d52c09389bd7bed59a0346fec3b5a3c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:20-ea-11-jdk-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:365b2235b36497d8797ac86bfd8e896069c8e9744ca0952b5203b20dacdf88fb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.3 MB (299290872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd3d39159c3faba5f5174b1001a1366f72dd096095f3360a4d110a66ac3701c`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:00:08 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 Aug 2022 17:00:09 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:00:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:00:18 GMT
USER ContainerUser
# Sat, 20 Aug 2022 01:56:21 GMT
ENV JAVA_VERSION=20-ea+11
# Sat, 20 Aug 2022 01:56:36 GMT
COPY dir:2a36fd13b231cb04e1ec355b8dba1ad544ab0672d28559422af08c676d4a6345 in C:\openjdk-20 
# Sat, 20 Aug 2022 01:56:52 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 20 Aug 2022 01:56:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151c855f0d179e8547473b92e962fb22b468853448fe0849dadde3526c52aceb`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3386f9f9687d0a909a16379459e37c52a2de2070297d81d4167037a0602e3e86`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092505f98fc516238306cba539a3a8a6d7f48ca19dc6e6c3cca668dc6f466c`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 75.6 KB (75615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfea14a612ecceac1dd16eaa1da4863923aa41d796fd4f9c1fae46d918d4299`  
		Last Modified: Wed, 10 Aug 2022 17:28:33 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ac953c4950d7b17d571b2e932558b6f6fd88c0fa2350cd324e1e621fe0e1ea`  
		Last Modified: Sat, 20 Aug 2022 02:06:52 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b179dee3f2205b23de6d816c617e6d8c150a27e613046c846c0caec18c7ab2af`  
		Last Modified: Sat, 20 Aug 2022 02:07:14 GMT  
		Size: 192.3 MB (192284817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f10c52ffa295a954e7d1b060f59acd58c6e569fe317de72e0403d436e7929a7`  
		Last Modified: Sat, 20 Aug 2022 02:06:53 GMT  
		Size: 3.7 MB (3719601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f50f0ec16be70a59092609f402182d7fdbe2ab62867514cc0a1ec88a1f7283`  
		Last Modified: Sat, 20 Aug 2022 02:06:51 GMT  
		Size: 1.0 KB (1029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
