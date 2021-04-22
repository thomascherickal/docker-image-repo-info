## `openjdk:jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:4ed92c14afc9c1771c409107ee6919b4d42759c7ce2af29c9180f36911ad23d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:jdk-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:898297a09b39c0d6558177560a035a3ac6b34bc69b8c8d261c24a2eade516e10
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.2 MB (285182577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:249324e98cc05ac10cef1ef164c90293f079c296de71d33c620c9b94786acfa3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:53:40 GMT
SHELL [cmd /s /c]
# Wed, 14 Apr 2021 17:01:24 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 14 Apr 2021 17:01:24 GMT
USER ContainerAdministrator
# Wed, 14 Apr 2021 17:01:39 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Apr 2021 17:01:40 GMT
USER ContainerUser
# Wed, 21 Apr 2021 13:07:41 GMT
ENV JAVA_VERSION=16.0.1
# Wed, 21 Apr 2021 13:07:58 GMT
COPY dir:ec453f8f02d21eabd8383c9d68e7e854c44e602cce3510b820d8ac55a0745712 in C:\openjdk-16 
# Thu, 22 Apr 2021 07:47:55 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 22 Apr 2021 07:47:56 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c2c727299531adc7c2aacb1f062d72fd42cec96a0d235b3e5b0afe03e9ddbc7d`  
		Last Modified: Wed, 14 Apr 2021 17:41:13 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d8da3586de7160296948acfffc7e4146122a7dff913ba7d3a9dcdd69de8627`  
		Last Modified: Wed, 14 Apr 2021 17:43:19 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4525b9aff55d1268eee10fa04063e7bc4c375329cf1aab32caecf1915cb566a5`  
		Last Modified: Wed, 14 Apr 2021 17:43:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ba7774e6e0c9f46b40c23675b77e86192a71b8fb2295614bb08b7aa8bbbb37`  
		Last Modified: Wed, 14 Apr 2021 17:43:19 GMT  
		Size: 67.3 KB (67288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8b8ae9e0cac207d383dc46c4887e9f40af304da4dd1adcb66cb9c2ab8821ce`  
		Last Modified: Wed, 14 Apr 2021 17:43:16 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461226b2bd9c5991e6bbfcb5b9bfa8bc742f5644b0461be44f85846d8c2f746c`  
		Last Modified: Thu, 22 Apr 2021 08:47:59 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0174cfcf443331d1707bc276cfdda1cabdb94fd10d924a69e2839130abacba45`  
		Last Modified: Thu, 22 Apr 2021 08:51:25 GMT  
		Size: 180.1 MB (180079750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65deca9ad3dedeba255bc2fed0d3f8dece0114dbf4a2d429954ac1ac96afce40`  
		Last Modified: Thu, 22 Apr 2021 08:48:04 GMT  
		Size: 3.7 MB (3688436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de06dd8eaf14c556db5a44bf3d36ef79621d01788fba5ae42a3a237e9b32f78`  
		Last Modified: Thu, 22 Apr 2021 08:47:58 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
