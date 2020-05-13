## `openjdk:11-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:9f78b17189b29a8df0dcd505e1397ca975d8d5d094051d46867a77e2d665f97d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1217; amd64

### `openjdk:11-jdk-nanoserver-1809` - windows version 10.0.17763.1217; amd64

```console
$ docker pull openjdk@sha256:1e3e9d5c997f3859170bd193913662cc02cadc4726d9eaaae70408492829666a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.1 MB (291137156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7fdfee15670a55f445daeead398088d0061be4440f946cd555e7fde2617e8a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 May 2020 12:39:06 GMT
RUN Apply image 1809-amd64
# Wed, 13 May 2020 15:30:41 GMT
SHELL [cmd /s /c]
# Wed, 13 May 2020 15:46:45 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 May 2020 15:46:47 GMT
USER ContainerAdministrator
# Wed, 13 May 2020 15:46:58 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 May 2020 15:46:59 GMT
USER ContainerUser
# Wed, 13 May 2020 15:47:00 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 13 May 2020 15:47:51 GMT
COPY dir:d90d60e1c0505496926373a51cab7b6b2c4fc0bb30d14b79fe3ef70ac0ba6a6a in C:\openjdk-11 
# Wed, 13 May 2020 15:48:11 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 13 May 2020 15:48:12 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b9e6fec25718aef5ed18d499b27e43adb524f9ee4f2eb3f0fffaea018e7e86b0`  
		Size: 101.0 MB (101019852 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c597e8fceaeb76628095f6dcfa538d497e85739068a817b45d73be2b96a3b37`  
		Last Modified: Wed, 13 May 2020 16:09:16 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a03dcdae6cede6a75edb6fe3889a452ab70bbd6e136d6f0d207f7a9411c675`  
		Last Modified: Wed, 13 May 2020 16:21:22 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455c55df9c9e2f5031f91b9d2f71a1bd776b848d02f8731afc41917d19415e8d`  
		Last Modified: Wed, 13 May 2020 16:21:21 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4321f6d5071190df54c60d08e3e0d900ce8e9db6837d9d32d391479f93062`  
		Last Modified: Wed, 13 May 2020 16:21:21 GMT  
		Size: 70.6 KB (70620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde052b3a9869d30319f8de12736294b1ea52c5a77fbc66cc2e5a057eb59409a`  
		Last Modified: Wed, 13 May 2020 16:21:19 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e216f310e3f3a8a4b738baa8599cdc907f13085e26f6f17bae5c10826b0fafb`  
		Last Modified: Wed, 13 May 2020 16:21:18 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a92304b0c81f51b91d87fe9dde4779d1b58bf54f18c3543ca2f704c1798254`  
		Last Modified: Wed, 13 May 2020 16:24:39 GMT  
		Size: 190.0 MB (189976192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1067d8af29aa2c0c25e43050ba129aca8068de8a0147dce64d46228d65c79b`  
		Last Modified: Wed, 13 May 2020 16:21:18 GMT  
		Size: 65.2 KB (65225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e919764a0db5c7044027f79df29cb6c61dd47fd29a2d5477767cb2cfbc89adf`  
		Last Modified: Wed, 13 May 2020 16:21:18 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
