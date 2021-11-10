## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:14c03718e7a3b5b4d6e904ec8dd76c7b6cd6cfa8acf175cab9fcf1ebd1842ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:04721a9682603edfb9fd2bb54ffeaa16d7a4b90d8fc0696dbe1d33ca829c84af
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.7 MB (145670605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d46691900a1cda57a4c27388694a18c916f0f4d5593d21f538fa6c773e55fa8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:27:14 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 10 Nov 2021 17:27:15 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 10 Nov 2021 17:27:16 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:27:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:27:25 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:34:32 GMT
COPY dir:6031cfac1e4bd8de6c5533bea0aabc25715779d854db7f41b8aea3e1449ff0bf in C:\openjdk-11 
# Wed, 10 Nov 2021 17:34:43 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e60ec86b90e1492e0e0ed2cbebcf624990a34862e24207343fd85b84b3544c8e`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77abcc84b1fe0c0732a70981bc9d18fa99841caac8f28e8d2ecb4e3a4c3c026f`  
		Last Modified: Wed, 10 Nov 2021 18:16:52 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97945d1b1c985a8d91d7b28f66d94a057114fb274bc6dc4c0ede17f6c929b4a7`  
		Last Modified: Wed, 10 Nov 2021 18:16:52 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f934df860a9f82c972e7c34459be16376c564aa0230d8267aabc7e04d196cc8`  
		Last Modified: Wed, 10 Nov 2021 18:16:52 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ac38e53fe15e27e522b84ccfac7f965b20337081c23a4950b20d3022dbd12f`  
		Last Modified: Wed, 10 Nov 2021 18:16:50 GMT  
		Size: 70.0 KB (69958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd4c7b5ac21d23163372736c624a9aef2e053864d031427007c61daef8fb06`  
		Last Modified: Wed, 10 Nov 2021 18:16:50 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62c81fd379d905e18ed9e514400cce74b6c9c975f69a3fa2824a94711ea8477`  
		Last Modified: Wed, 10 Nov 2021 18:30:10 GMT  
		Size: 42.7 MB (42723341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff9d3ff32b2e62752d4e2f868520a2dd2c40f44f4e4717ecb5617139914b9d4`  
		Last Modified: Wed, 10 Nov 2021 18:29:23 GMT  
		Size: 88.5 KB (88548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
