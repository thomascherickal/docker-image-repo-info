## `eclipse-temurin:8u312-b07-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:580f2215d015f52831a1906ab70db257ce602a591892a5eeebea2dc7ad956f39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:8u312-b07-jre-nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:a0fc26b7c4e001dc87f56134e891782ad6569ff5350d1b775d26d74753bd64e1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.4 MB (156372318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e12878914b71d8e05daf18415e032ee51bfe97b7ee96b9cec0a7ab6206ac379`
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
# Wed, 10 Nov 2021 17:53:15 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:53:28 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:0eb61e0c01de5c281535eb310414e9aef8bbb926d6f7beadb9c476047209bd3b`  
		Last Modified: Wed, 10 Nov 2021 18:54:25 GMT  
		Size: 39.1 MB (39081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a65665d9dbd44743f8aaeeeeb8e7600716fce59cf6257b2c5a1c156dd8200`  
		Last Modified: Wed, 10 Nov 2021 18:54:19 GMT  
		Size: 68.6 KB (68577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:8u312-b07-jre-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:cbfde24c2160b85ff37f85c1248a57840ce851f8248e0f7055c401efc28c5d1e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (142028689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7740d3c9b06407bcd433db3fa7d008a36e54c06c11ab9dc195566a8d05a80085`
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
# Wed, 10 Nov 2021 17:20:04 GMT
COPY dir:f43ebde5893522b38a147191e5e447aa435ef67c7d947aeb3e536f25bc61cdb3 in C:\openjdk-8 
# Wed, 10 Nov 2021 17:20:15 GMT
RUN echo Verifying install ...     && echo java -version && java -version     && echo Complete.
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
	-	`sha256:372d5c385299de41e8b2e83a8f82cc7f8384050b97d40a496fd5c516f87de204`  
		Last Modified: Wed, 10 Nov 2021 18:07:46 GMT  
		Size: 39.1 MB (39085423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07a70b6f600a1de32d16839283d37efaa5f80c61c5cdc130b1a22b66073cead`  
		Last Modified: Wed, 10 Nov 2021 18:07:41 GMT  
		Size: 86.3 KB (86322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
