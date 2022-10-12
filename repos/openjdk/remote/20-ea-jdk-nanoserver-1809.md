## `openjdk:20-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:27e1b5141e682a3d680317efbec9d18703d04c6552a736c953a49237ef3de00a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-jdk-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:82a835cb33cb28b0e66d573ea529eab9d919dea344d4ecf1febe492d1624586b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.1 MB (299133293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c652ce87db6e1dea7a6085c30d7985560778a17459a172263bbacba039ee53cf`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 15:20:49 GMT
SHELL [cmd /s /c]
# Wed, 12 Oct 2022 16:43:51 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:43:51 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 16:44:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 Oct 2022 16:44:03 GMT
USER ContainerUser
# Wed, 12 Oct 2022 16:44:03 GMT
ENV JAVA_VERSION=20-ea+18
# Wed, 12 Oct 2022 16:44:19 GMT
COPY dir:483e8c5e7a9f569d5f056ca40e9cc5008b7d0f5f9a8d61a265181e1e2313d355 in C:\openjdk-20 
# Wed, 12 Oct 2022 16:44:33 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 12 Oct 2022 16:44:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5ead999142ecce15e02523c49706a633fa708374d94bb65a254e3a3c117d609b`  
		Size: 103.4 MB (103377244 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a6a667d76c19fca171390d60fb90c40e16c777050e943a7fe17ad7686841f0f`  
		Last Modified: Wed, 12 Oct 2022 16:02:59 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4315d417eb7958a05c7977d0ea6b1b4745e46725d02f23235173bbad2c73101d`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c783713d738fc9dfff161ad3ff4369333cd0881466ab886feb09e6ef3508512e`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05686fefb2145f84031cd9cae616dd90496d078df87f19c080931972eb700e7c`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 67.2 KB (67186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab8462cae193737dba91e48900abf79d1b7234b48f337497ae0abfe9d8189e5`  
		Last Modified: Wed, 12 Oct 2022 16:53:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d6beb7bda80b5ded6a78a8dd7a195469e6344b84e9b6fbacd6b198de5fb05d`  
		Last Modified: Wed, 12 Oct 2022 16:53:07 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc06c3f515bfdaac758d6c8219f598234c4a17750a239e5ea5fd155d9aaadeca`  
		Last Modified: Wed, 12 Oct 2022 16:53:26 GMT  
		Size: 191.9 MB (191929365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7106596b2bd97b570a449461227a198c521dd4ea986ea1ba8aff8a5c7d93a79`  
		Last Modified: Wed, 12 Oct 2022 16:53:08 GMT  
		Size: 3.8 MB (3752550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac38627cd3681c822ecc0b6fcd1acea3245dd30405d9387a571b0879809ec6`  
		Last Modified: Wed, 12 Oct 2022 16:53:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
