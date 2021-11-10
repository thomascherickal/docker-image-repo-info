## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:3a01d4fe7dc2d8612062228129c77222d2f4b15dcb61be03b82cedb7939549ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:44da197bab07f2ee040d23ebe0370d543fa485af7261eb983ca9c2c5127e599d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (159988563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60dfb531f7352aa139f0e2a1377ed2d6b253409fa34a8b9967144de38db2b380`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:53:35 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 10 Nov 2021 17:53:35 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 10 Nov 2021 17:53:36 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:53:45 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:53:46 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:54:34 GMT
COPY dir:6031cfac1e4bd8de6c5533bea0aabc25715779d854db7f41b8aea3e1449ff0bf in C:\openjdk-11 
# Wed, 10 Nov 2021 17:54:46 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e60a18aefb5c5bb8955067d23b9a2f7d1157a88831ce6b2071cec8e581f077`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab70470578cfb024d7d073a90446e09fa7f464faf9d307a6600607d8c10471b5`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a719fea5e976f3229d956e7e3371e962995af4e615fa7a7badeac24443be7`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796f2ca8a54d4f8b5df8581be27e1229d8ab11142cc1a1c26e47c15f373122d`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 83.5 KB (83528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5bee5015e8ba92e3c8630de1842c7e17dec954ce3d3ce5fc2a769042c2792f`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd2354f399d602ff73218763439e0788c810968374e77e4588f645809aff0ce`  
		Last Modified: Wed, 10 Nov 2021 18:59:03 GMT  
		Size: 42.7 MB (42720673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788c578872591287c7cd5dc8d6ba5ce3805326ab7e2adb836fbd464bf6746db4`  
		Last Modified: Wed, 10 Nov 2021 18:58:15 GMT  
		Size: 61.8 KB (61801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.2300; amd64

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
