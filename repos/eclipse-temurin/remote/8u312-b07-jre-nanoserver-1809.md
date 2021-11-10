## `eclipse-temurin:8u312-b07-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:07a39049eabc73533b96731dfd38c0df6b537cdd26da6a656b2975023fbf2cd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:8u312-b07-jre-nanoserver-1809` - windows version 10.0.17763.2300; amd64

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
