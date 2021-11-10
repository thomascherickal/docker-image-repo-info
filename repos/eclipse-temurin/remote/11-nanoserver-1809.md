## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:d764c8ee5ce3e0aebe7da536e698b4ac688708d7517fc31414e998746e287bcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:dbe93d723df8aef49d7d01b97d7c0e977f905c4aac06db91ab2a05819a23554c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.9 MB (294890364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3b0211e4616f9b1503146d24a5ebabcc3d109d78902be54f528ec40286acbf`
-	Default Command: `["jshell"]`
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
# Wed, 10 Nov 2021 17:27:40 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Wed, 10 Nov 2021 17:27:51 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 Nov 2021 17:27:52 GMT
CMD ["jshell"]
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
	-	`sha256:bbc517503fa735971352d3efd512025f4aa23268f10171044a47427575ed1770`  
		Last Modified: Wed, 10 Nov 2021 18:20:22 GMT  
		Size: 191.9 MB (191947483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ed461f4da1053d74e19128161a5179a0450b767a84478c7e738a114c88cf37`  
		Last Modified: Wed, 10 Nov 2021 18:16:50 GMT  
		Size: 83.0 KB (83039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7427e5fab3baf7cab0d8c659c0b2af78daad638ee110b4fb30ef2d0c406e44`  
		Last Modified: Wed, 10 Nov 2021 18:16:50 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
