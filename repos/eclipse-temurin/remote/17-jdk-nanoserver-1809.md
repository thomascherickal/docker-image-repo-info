## `eclipse-temurin:17-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:7de7f5f6751ff5c5b1ab4a0e16002ce2adfbc79f2421123d19117ebcab64dc1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `eclipse-temurin:17-jdk-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull eclipse-temurin@sha256:8b2d567b88290958c2755f113614eff25293e934a773c18e50d2a0ee88fef6ca
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.8 MB (291810499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77ca5afc041ad2b41de186bfd51eb918f58ec90eb59c21eda662597a0f8891f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 21:56:20 GMT
SHELL [cmd /s /c]
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_VERSION=jdk-17.0.2+8
# Tue, 08 Mar 2022 22:20:39 GMT
ENV JAVA_HOME=C:\openjdk-17
# Tue, 08 Mar 2022 22:20:40 GMT
USER ContainerAdministrator
# Tue, 08 Mar 2022 22:20:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Tue, 08 Mar 2022 22:20:54 GMT
USER ContainerUser
# Tue, 08 Mar 2022 22:21:08 GMT
COPY dir:af72ba1102e9cda7f5ea9974b0cafbe96b2f97690adb0743202a1c732a987a84 in C:\openjdk-17 
# Tue, 08 Mar 2022 22:21:25 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Tue, 08 Mar 2022 22:21:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e0065cd23a657c8f30ae5af121fd18451d2307835a1124ea57c80683eda26c94`  
		Last Modified: Tue, 08 Mar 2022 22:37:21 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e28e0120ae71480ac4b5292e1011f3e9a68e7648b992c086019524244ffc7f1`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d91688edda3231dbafc3286e5ecd7bcc1653c6a0e16cc01372b62928a409ef`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2195699d328d0527e400e78f2794d1150c371b24ac84f8bf12bba4aa47e9c2`  
		Last Modified: Tue, 08 Mar 2022 22:50:04 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b8d01d40707a79981646b757c4bb673b5163d48f0f7e69f846dc526b2f5236`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 72.2 KB (72220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759cdd0f2650d033acdd0769c7ca2cf4ab535325556e99d303605abfbcbaccb0`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 1.1 KB (1118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59910ceb582f292b3d99a9ead8c18861be781eacb6b20f4af1a91d3055b14855`  
		Last Modified: Tue, 08 Mar 2022 22:53:41 GMT  
		Size: 185.0 MB (185014542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075a8361190c5a48c70964b3f48a37a8447872b33dd2a9334ac25247be1e0a77`  
		Last Modified: Tue, 08 Mar 2022 22:50:06 GMT  
		Size: 3.7 MB (3662324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd82e86e89538af4a39f52d5c5f340dd8befbf67fa8d3ca19df0ac958a5ff2bf`  
		Last Modified: Tue, 08 Mar 2022 22:50:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
