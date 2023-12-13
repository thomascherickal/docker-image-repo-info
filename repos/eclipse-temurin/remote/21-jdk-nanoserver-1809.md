## `eclipse-temurin:21-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:ecae1a43f2b6685c5863643e24805c883d5877f222a85a883960b40c62a3f292
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:21-jdk-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:f3c31bf3c42d7cfa3ded01e9fc8029898e17e5d9c9a9aa4257558ecdeef37c4f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309400456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f521f934844773db00837633c7b5def025bc0453c87e6a6ac26b417965253116`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:43:51 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Wed, 13 Dec 2023 00:43:52 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 13 Dec 2023 00:43:53 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:44:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:44:01 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:44:14 GMT
COPY dir:fd62014fea6b5cd8b6f3d34ff8f9c5e95aa0ce969b7fd9201e979e77a3abe050 in C:\openjdk-21 
# Wed, 13 Dec 2023 00:44:28 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Dec 2023 00:44:29 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e210dfff18c7fa8686391936abc0d2af8c9be07425284d44eee4bd71393f38`  
		Last Modified: Wed, 13 Dec 2023 06:42:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b6b3c445f2e422cde82689d67928307c430e51176ddc0a5285099109fa8036`  
		Last Modified: Wed, 13 Dec 2023 06:42:49 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a39d2429e9e771dcaacf3c869673b184529fe63613fde8ccd522463eed06cb2`  
		Last Modified: Wed, 13 Dec 2023 06:42:49 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28f2d00f5617e4a3cac5f05d95d52f8fb2eeaf1a627a394cc494b54d86686e`  
		Last Modified: Wed, 13 Dec 2023 06:42:47 GMT  
		Size: 68.2 KB (68210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d5852a4d2b878e72b61e9938d2735a9c628bc461d4f55e9ec2f613f3cdf2e`  
		Last Modified: Wed, 13 Dec 2023 06:42:47 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168a2012d8a0c481d26e32d40d402f690fb6f89cde92f8569446677919911283`  
		Last Modified: Wed, 13 Dec 2023 06:43:06 GMT  
		Size: 201.0 MB (200995873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be91bd0bf396771523b7fc9c143c7408999d011a96d668995b2503c23c52a3f2`  
		Last Modified: Wed, 13 Dec 2023 06:42:48 GMT  
		Size: 3.8 MB (3819374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8a82e8f7121ebc889abb5f37e8324ce003933a587a84de175b37eac2335105`  
		Last Modified: Wed, 13 Dec 2023 06:42:47 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
