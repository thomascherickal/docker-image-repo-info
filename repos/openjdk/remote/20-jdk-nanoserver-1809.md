## `openjdk:20-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:8792ffc1c8f6333503b1da9462b5bd6fa4dd548bfb9cd7d7eea766b5c92ea6f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `openjdk:20-jdk-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull openjdk@sha256:a16a2bd6aba51be91f4d1af9b6c01af086231d651d97cb27a9326b1d99432cd2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (298971952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8f1b6d59cd6da986d0604e4eb67a64ae6f5533d613cb777eca86be3b595059`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 16:03:00 GMT
SHELL [cmd /s /c]
# Wed, 14 Sep 2022 17:08:57 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Sep 2022 17:08:57 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 17:09:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Sep 2022 17:09:07 GMT
USER ContainerUser
# Wed, 14 Sep 2022 17:09:07 GMT
ENV JAVA_VERSION=20-ea+14
# Wed, 14 Sep 2022 17:09:23 GMT
COPY dir:fc970cad6b623d3dc96cba13e483a4ee274232db202104df6c8122d640a77515 in C:\openjdk-20 
# Wed, 14 Sep 2022 17:09:37 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 14 Sep 2022 17:09:38 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:233f09b2a52487084f2cfb5e06dac2815651432c9d37c729582f59cfcf66b243`  
		Last Modified: Wed, 14 Sep 2022 16:47:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f67cb607010c6768708866762c8f245af049da7669af90242ea7dc3d1881f80`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd0c7e3fefcb9d81347f1ab494f4177ae8fff7d71ac827f5e90d34ee4bf483`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72046412150cabb4b6b5ba4cf56188800073ddce5f570b7d921bc62eb13c577`  
		Last Modified: Wed, 14 Sep 2022 17:22:54 GMT  
		Size: 67.8 KB (67836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea99aee812db540f38ee961b7634ec0afe7d8468d85e3adaabe234fee1414d5`  
		Last Modified: Wed, 14 Sep 2022 17:22:51 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e382e34b500752bc3d6cbabd5a84a5778841df2a4c3600850d0f5de973e886`  
		Last Modified: Wed, 14 Sep 2022 17:22:51 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2b6aaf17a39e01e210d0b7b7412cc70faa097dd3afe83023ec04d79e3ade0c`  
		Last Modified: Wed, 14 Sep 2022 17:23:12 GMT  
		Size: 191.8 MB (191814811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67eeaf9281919b55605d34833d515e3299c72943a963a7eda21f8c27c0092d2b`  
		Last Modified: Wed, 14 Sep 2022 17:22:53 GMT  
		Size: 3.7 MB (3748234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accc6382ed4cdc43a54c5e8daeeb770b44ea8ef796b6af32673db4a3a8773c1`  
		Last Modified: Wed, 14 Sep 2022 17:22:51 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
