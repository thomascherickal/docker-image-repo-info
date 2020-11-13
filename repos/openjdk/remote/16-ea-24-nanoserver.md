## `openjdk:16-ea-24-nanoserver`

```console
$ docker pull openjdk@sha256:c4ba3201dbaae73dde41134948bace4d33d0eb71e713bc4c8d7f27402e61c854
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:16-ea-24-nanoserver` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:3b68fc6d590200a7175b27135d51608e7cc1702a42417bd177a7ffe21b21deb4
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.9 MB (283946400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4787896421c4555615a0562d31b316c9066cb930876ccd9269ef4233d6a68206`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 31 Oct 2020 05:10:43 GMT
RUN Apply image 1809-amd64
# Wed, 11 Nov 2020 17:53:16 GMT
SHELL [cmd /s /c]
# Wed, 11 Nov 2020 17:53:16 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 11 Nov 2020 17:53:17 GMT
USER ContainerAdministrator
# Wed, 11 Nov 2020 17:53:32 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Nov 2020 17:53:32 GMT
USER ContainerUser
# Fri, 13 Nov 2020 19:19:51 GMT
ENV JAVA_VERSION=16-ea+24
# Fri, 13 Nov 2020 19:20:26 GMT
COPY dir:64a1448e97a1a7e4b4b9601995d9e5eedf3833e9d164b8dda2ffaf5a0c17059f in C:\openjdk-16 
# Fri, 13 Nov 2020 19:20:49 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 13 Nov 2020 19:20:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f1b217fe8837d4d85cb8228a52344d3504d7aa51ba30167a20a6a4cb80cdcaa0`  
		Size: 101.3 MB (101279682 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:41b7be9dc08821cf81d29b16e0df54f7f3e3aeaa6407f43520c6259f2d84b10c`  
		Last Modified: Wed, 11 Nov 2020 18:27:27 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e637122599038842d743045a8ebfbfa35dbadf7dfee0adcc2ba903e891ab072d`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7fa5c85bf3c3dc79cf3bec9aba597aa0b5c38c234952da905e86d7a556b6f3`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 912.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9c6b451f516c5e78ab16ded450d01a2a45dd13d0cac12cb9b043f5d87f993a`  
		Last Modified: Wed, 11 Nov 2020 18:27:25 GMT  
		Size: 67.3 KB (67302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac0f27f5ace77a66a18d26e72bf8f24216110f8ed5b6f951597b9a42d3ae52b`  
		Last Modified: Wed, 11 Nov 2020 18:27:22 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df67bb08b7ea2c3d54f2689f41262f6024c6cb255a8b7791a6d9b9d8e23b95e`  
		Last Modified: Fri, 13 Nov 2020 19:26:03 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd7ea4e8049d9da370584ea3a7038b32a58d6fee0c1a5595906b0c06860aac`  
		Last Modified: Fri, 13 Nov 2020 19:26:21 GMT  
		Size: 179.0 MB (178966066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44424fa3370200f3a678c8bde6945b20b606a28993e0fa4bd2b3478ccc961d60`  
		Last Modified: Fri, 13 Nov 2020 19:26:04 GMT  
		Size: 3.6 MB (3628083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd07ae3af5b0f20c3a76669a462d470974b4e7fbb392a55acf6c2aa48ba18f`  
		Last Modified: Fri, 13 Nov 2020 19:26:03 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
