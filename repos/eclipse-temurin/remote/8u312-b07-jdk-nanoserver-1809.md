## `eclipse-temurin:8u312-b07-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:88d777cc3b9d9104cecb397602b8de3ebbc9bb809508d2297011b5508ceefe37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:8u312-b07-jdk-nanoserver-1809` - windows version 10.0.17763.2300; amd64

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
