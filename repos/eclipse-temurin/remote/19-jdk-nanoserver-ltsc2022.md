## `eclipse-temurin:19-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:a27f56ceb9e499004a17fcdecacfe1d04071b53a48c404dd4bca3194dcd2b4e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1547; amd64

### `eclipse-temurin:19-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.1547; amd64

```console
$ docker pull eclipse-temurin@sha256:18064bf0a5871c834d45da587025fca0418202c2530cc967283c29652b5d6027
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.6 MB (315568914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43aa84433f5c2201b7f5b1db5c804f47e2a4f84b2fb34b47b3ff3651b7b7d7d9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Wed, 15 Feb 2023 23:34:03 GMT
SHELL [cmd /s /c]
# Wed, 15 Feb 2023 23:39:50 GMT
ENV JAVA_VERSION=jdk-19.0.2+7
# Wed, 15 Feb 2023 23:39:51 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 15 Feb 2023 23:39:53 GMT
USER ContainerAdministrator
# Wed, 15 Feb 2023 23:40:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 15 Feb 2023 23:40:05 GMT
USER ContainerUser
# Wed, 15 Feb 2023 23:40:22 GMT
COPY dir:09b3ada3bc8ac44822b97a9a56d697461744d2194cdcb6ab15233b0b9b376e38 in C:\openjdk-19 
# Wed, 15 Feb 2023 23:40:55 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 15 Feb 2023 23:40:55 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21b41cddbbbe3e6e7b8691f9cfc05eac50290ddadabfd44482b251564c6481`  
		Last Modified: Thu, 16 Feb 2023 07:21:04 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab91262862cc0e1158f4869edf93e820c80fe8cc5360acef90052f4d26d837e5`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58929160bedb85968bc7fd10c682785c2a1ac5f89d9d2736265bcb99196a55cc`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea29e5d115afd492396980741a4cfb3b8d1d12df5c7887739565ac1234ea0f6`  
		Last Modified: Thu, 16 Feb 2023 07:23:45 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83afce58205f8116dc64c080dd9ef9502447b4c292108bd5fba82c1e9b19f546`  
		Last Modified: Thu, 16 Feb 2023 07:23:44 GMT  
		Size: 83.7 KB (83726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9d476cdc226464e55897a95ac3eda65bf7cac4ff190da662c7525c31b898b7`  
		Last Modified: Thu, 16 Feb 2023 07:23:43 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af8a932f5418da9fb3a7a2b0f121c4eeb3bbc9100c0c2175746b229c44ea77b`  
		Last Modified: Thu, 16 Feb 2023 07:24:09 GMT  
		Size: 193.3 MB (193268078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225bcd252e6e37d23c4e3ed2e9dba5f1977db7506866d98cfecfc82bf389fee9`  
		Last Modified: Thu, 16 Feb 2023 07:23:44 GMT  
		Size: 91.0 KB (91042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b317ba1d4c29ba54d05d495b1effc4203be78bc9037fac35038edc1e5ed3fdd4`  
		Last Modified: Thu, 16 Feb 2023 07:23:43 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
