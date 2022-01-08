## `openjdk:18-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:de3268427112be4cd7ded9a64515fa6f2b8dd38e501f0c350f9356a1de86ce4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:18-ea-nanoserver-1809` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:1f7add64587c6653ae15dec5bc6d86353ef4e336d378d73762735c8ae46b7fd3
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.5 MB (290497444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c212886785a0e8859a0e5bd22f26a9b57a34b131d8df71660739050edff0da62`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 05:18:44 GMT
SHELL [cmd /s /c]
# Sat, 18 Dec 2021 07:11:41 GMT
ENV JAVA_HOME=C:\openjdk-18
# Sat, 18 Dec 2021 07:11:42 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 07:11:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 18 Dec 2021 07:11:54 GMT
USER ContainerUser
# Sat, 08 Jan 2022 00:57:32 GMT
ENV JAVA_VERSION=18-ea+30
# Sat, 08 Jan 2022 00:58:03 GMT
COPY dir:3d6861a7fa55c63d29eac691cb55df2ed4bfbbb831002267ccd0f83773649293 in C:\openjdk-18 
# Sat, 08 Jan 2022 00:58:20 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 08 Jan 2022 00:58:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4c557aac927613dd487d7c04b01a8eeb8ad174693f61b14c8f4285f1db6afdd2`  
		Last Modified: Sat, 18 Dec 2021 06:13:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb09a08117aed517f83acd09c46245354fda9e1f94c432b6c5be4758bd11846a`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9558b80b57be79d231423f31ff119a52bfde5373d41866669b3536cad1fe939`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f711c3cc04e41a513139b9dce135ea0dc407bb92c80b5fb14341e73eca8e7`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 67.3 KB (67275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8203006c00a339abd7dace4c1b632bcbb99479c9cbd36cdf65f5ca4363d6872d`  
		Last Modified: Sat, 18 Dec 2021 11:08:05 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d241a5cee749ed0f0fb602b2416993df0773f8fd2fde88987db981730161bd0`  
		Last Modified: Sat, 08 Jan 2022 01:11:46 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b38e545fb38e80b52d59b021f9307266ba066f2c4adcf16c3e92c8eeff7556`  
		Last Modified: Sat, 08 Jan 2022 01:12:06 GMT  
		Size: 184.0 MB (183979267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346603e9512a5874d819b7e007ffcea123747b09e1254fca87651665dea03d2`  
		Last Modified: Sat, 08 Jan 2022 01:11:47 GMT  
		Size: 3.5 MB (3539915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea92645bfb8a075ea818b1d0137125b4e405bb4185a02085b78ba313e431b65`  
		Last Modified: Sat, 08 Jan 2022 01:11:46 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
