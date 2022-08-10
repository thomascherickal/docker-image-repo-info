## `openjdk:8-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:a616cda38559dc7fae5c195de793287f62486c00813bd54b937e60991a474db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:8-jdk-nanoserver` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:391eb3ff409f71545ccfca38da6fe33a5a7fb92a58dd5cdad61e6c1cfa6e811e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.3 MB (204314674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78359b2b86bc82cbb5eda6adb577c8814df12dc20059d6924d994d1191ba0024`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:21:14 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 10 Aug 2022 17:21:15 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:21:24 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:21:25 GMT
USER ContainerUser
# Wed, 10 Aug 2022 17:21:25 GMT
ENV JAVA_VERSION=8u342
# Wed, 10 Aug 2022 17:21:38 GMT
COPY dir:9c3bba9710713dbb55751ce63d59239c9d60548d5128ebf71c30f559bc754473 in C:\openjdk-8 
# Wed, 10 Aug 2022 17:21:51 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6f03744b411c834fff8541b86c417dd9cebbbfd149ea75944e3d1c8766aa8e`  
		Last Modified: Wed, 10 Aug 2022 17:37:33 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e306e6fe26dd8faac775af256f32982b10533d20c3781942b4e464ea13493b`  
		Last Modified: Wed, 10 Aug 2022 17:37:32 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d005dbf9dda3bf691f799d207ea911cf138f23df57a88ec12b25dd874ad854`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 67.6 KB (67569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e58525a260d7308aeb21e49035b7588309aae8b4fe37c17563ea45ba947028`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ba3f94dcb65edc82c61f421dc102e7dfd352a8a761de9992c40fdb23dc3018`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3cc96ae7c24beb01e1e666db7cb9734549bcc6ce890f899f736196288d5bdb`  
		Last Modified: Wed, 10 Aug 2022 17:37:41 GMT  
		Size: 100.9 MB (100949821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bca201c3f239305df30d4027517d27b3bfe5ea2e6266570abe4e0dbb49bb3f`  
		Last Modified: Wed, 10 Aug 2022 17:37:30 GMT  
		Size: 87.3 KB (87318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
