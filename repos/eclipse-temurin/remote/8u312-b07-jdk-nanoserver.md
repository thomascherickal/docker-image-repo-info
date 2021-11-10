## `eclipse-temurin:8u312-b07-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:bca4fb5714541d12131d8a24be921af2e34f7147a5ffb911d79be51bf07bfcb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:8u312-b07-jdk-nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:bca3801c0736a4cf5823f428170088083c9764db5066d3c7b312321150fd4731
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217482274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a2a5f5a4c5b0c9f9f0df086acae7a3ca1431a49626374b545644d8e41303e5`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:52:20 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:52:21 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Nov 2021 17:52:22 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:52:35 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:52:36 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:52:46 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:52:59 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ceb9b6cf720f75473e3c41307d287700ff9e2fcbb1e7fd036ed7a78a6c64e4`  
		Last Modified: Wed, 10 Nov 2021 18:53:57 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61655ff5d6ffb4e9b28c5bb62ef4e6838797460f0b1136f043b2cd0599eb5190`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8f8ab0cd19e99cc99b76ace65f501d956fbb5509b9973f1a12056915e44440`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52fd3b2829a4a90396e730bb05b5685ca3e796a913593b91dda4cc283e5e8b6`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 99.2 KB (99243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1743a12c5b583262adb490179aeb5cb182f8fe9389663880f95527c27db067`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fca1206701ed80928b003456c51993e69bad74253efac7e0f64eed25375c7a9`  
		Last Modified: Wed, 10 Nov 2021 18:54:07 GMT  
		Size: 100.2 MB (100190494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8134f2eda537f35a9812d6e63e9b42b621503bf8e4f06a3027e74331c7e373`  
		Last Modified: Wed, 10 Nov 2021 18:53:55 GMT  
		Size: 70.0 KB (70002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u312-b07-jdk-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:73173b8f4f1c45ccbe09375f805573659b2633176766e768d2f9bf7f1e0363f2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.1 MB (203134774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0708de34c11426eac01cf9045beeccd60630cb8c7ad2d0a911f335ffd314111`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:13:21 GMT
ENV JAVA_VERSION=jdk8u312-b07
# Wed, 10 Nov 2021 17:13:21 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Nov 2021 17:13:22 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:13:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:13:33 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:13:43 GMT
COPY dir:7d20e7860b874019800a6393f3930849559cf997f64b86d2d0263d858293fa37 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:13:59 GMT
RUN echo Verifying install ...     && echo javac -version && javac -version     && echo java -version && java -version     && echo Complete.
```

-	Layers:
	-	`sha256:b9dc943b4e8df8f472d444248152fa0920172ec630a60ada316e1603600dd1c7`  
		Size: 102.8 MB (102782944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e60ec86b90e1492e0e0ed2cbebcf624990a34862e24207343fd85b84b3544c8e`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0a598fb8138d98575ea500015d6bf1bd4c02a9084a0acd764cc14320adb868`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37fa4e74fe0fda0aeaadd37fb076fb079451999a04d605a2dfd1873bdaf0c15`  
		Last Modified: Wed, 10 Nov 2021 18:01:59 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dacb499c025b359d46120434faaa9e1f600b13c0bece257d24ea3f7538ecea`  
		Last Modified: Wed, 10 Nov 2021 18:01:57 GMT  
		Size: 1.1 KB (1095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe5850728b7feff7158a43bd822967023b9ad3d5806a24f287da3cf0addec09`  
		Last Modified: Wed, 10 Nov 2021 18:01:57 GMT  
		Size: 68.3 KB (68296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09b9935d0518c86f94599c78b87e69485930e711752547e4331711af691886e`  
		Last Modified: Wed, 10 Nov 2021 18:01:57 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1867617cb030558d801801c417fab4f444d973b0d420ad06b41afb20e009a9`  
		Last Modified: Wed, 10 Nov 2021 18:02:09 GMT  
		Size: 100.2 MB (100187640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7df126c789a15176a70337215c03409eb874b35e35bea2083900b37800a4038`  
		Last Modified: Wed, 10 Nov 2021 18:01:57 GMT  
		Size: 90.2 KB (90190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
