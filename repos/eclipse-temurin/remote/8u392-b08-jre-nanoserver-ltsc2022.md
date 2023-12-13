## `eclipse-temurin:8u392-b08-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:ac19d243b85ad6683064c4cdd68f0fc515b4c2439a75260877205560000fa08c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:8u392-b08-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:d47b06798930b4ba63caadf98b8abe31050df549e9fe73fb99ad8820a3cc72ed
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (161021802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d81ade2bb439eb37cba6f9160665059d17f8a2af3f4d14222d2f0d546cf021`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_VERSION=jdk8u392-b08
# Wed, 13 Dec 2023 00:49:13 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 13 Dec 2023 00:49:14 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:49:43 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:49:43 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:50:22 GMT
COPY dir:dbdf2dd9ed9894186d74b75beac1320724c73c6994b00118f04985f0ea2b3067 in C:\openjdk-8 
# Wed, 13 Dec 2023 00:50:34 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420e231f6e0404269e9ff487f0ffc079de3deb8c08e9ff31ccb5fda1d1a44ec`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf164bbdfb6f48a324b0a202412c204a0fe367efe5829ef14105bbd65605b66`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e516ed43c06e2b90a2550de28ed9e594a346fd4668e2807446ad69e0744fcd74`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaf7cc4c908cb1abf6fe51888bc260f997343bd25220752f0d3b86076713ae1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002dbdb57bb357c987be5ff6bcbc5e3cd108805d231b7f09809337c5f36e2ba1`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 85.5 KB (85519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2219f416115f1fbad27502353948edc25fab0d18bd677b2b058840104dbdc94d`  
		Last Modified: Wed, 13 Dec 2023 06:44:16 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193dbae1a56d927b5f1940dc1bc91493356eac659fb4abb8f955508b96da3b86`  
		Last Modified: Wed, 13 Dec 2023 06:44:44 GMT  
		Size: 40.1 MB (40111351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69fab786bcddc7d58783d4b2ef29b7431f2a40556c8a3f06eea6ea763c5b5cf`  
		Last Modified: Wed, 13 Dec 2023 06:44:38 GMT  
		Size: 62.1 KB (62106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
