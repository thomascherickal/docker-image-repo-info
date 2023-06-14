## `eclipse-temurin:8-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:8492396c041fc9459e7e07fc85dd43579c7048c0535d85e27adb67d6a51ba767
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:8-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:794e081c10c16fde8ad9bb0e8f8ffd94c43b24a7e9ae8f9cfbc01f691b3d7880
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.6 MB (221612061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31a8375bfab31cb1a0c93b71c84c1a1c00e95c5085d4bd6ab5ec6a511a500552`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:38:25 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 18:10:16 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 18:10:17 GMT
ENV JAVA_VERSION=jdk8u372-b07
# Wed, 14 Jun 2023 18:10:18 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 14 Jun 2023 18:10:18 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 18:10:34 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 18:10:35 GMT
USER ContainerUser
# Wed, 14 Jun 2023 18:10:48 GMT
COPY dir:27c7e47be02cf877d3f45f48fc9f53f313487829869ebfc4770f3f1b0ee2a0d5 in C:\openjdk-8 
# Wed, 14 Jun 2023 18:11:02 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:f94f5e4cef3f52c830328b87b7298c638fa9ef22a0babf737eda2a2dd6d024c4`  
		Last Modified: Tue, 13 Jun 2023 20:05:48 GMT  
		Size: 120.0 MB (120028549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b91974e610b0adc71baa1c4d1aa6d7a239880c5cef55dc0d33ffd0ef5ac9c14`  
		Last Modified: Wed, 14 Jun 2023 18:36:54 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf731e90fdff70f7b00179c7dd6369f299c0dc3a3f6b232cf4e53c524e14c174`  
		Last Modified: Wed, 14 Jun 2023 18:36:54 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5b58c506452b7a19fed03d32b461286862e3279405347d6ea9879c028a300e`  
		Last Modified: Wed, 14 Jun 2023 18:36:54 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20506f34863859eb158ae97aea15d3387f8313ac9a9140f39eccc869d3c50e88`  
		Last Modified: Wed, 14 Jun 2023 18:36:52 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8853ea636d657f5ff61f7ea74c38fb2f83d6067f98c1517d4df1d341ef1f7471`  
		Last Modified: Wed, 14 Jun 2023 18:36:52 GMT  
		Size: 78.6 KB (78610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39441605c531804ad4eab2f9055afe7db69607e0bfe09a80dab307bd3851d035`  
		Last Modified: Wed, 14 Jun 2023 18:36:52 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a207810ab4ff3cc5784462ccc2ba79380f3f910d1dc59d5b611cde6c802ea143`  
		Last Modified: Wed, 14 Jun 2023 18:37:05 GMT  
		Size: 101.4 MB (101438362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b832de6420319e6b5bb301ee4b242ee12cf66abff3d87442a9277005b5ae660`  
		Last Modified: Wed, 14 Jun 2023 18:36:52 GMT  
		Size: 61.2 KB (61188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
