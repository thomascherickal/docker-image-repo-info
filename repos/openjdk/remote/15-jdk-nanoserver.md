## `openjdk:15-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:2b6a3370b53242175a1fbc25f14c2331a009c293ea35f94caf824b6a6275f1aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:15-jdk-nanoserver` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:8bfc03608de3dd3f4fbfa5dd95b4a38d6f1966a5120afa0da53391776354d78a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295827532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6db59c4989a0b3140976478be9065cd3df12d26be52b9a1a7c6b64432c6051`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:03:33 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 15 Jul 2020 02:03:34 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 18:27:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Fri, 24 Jul 2020 18:27:58 GMT
USER ContainerUser
# Fri, 24 Jul 2020 18:27:59 GMT
ENV JAVA_VERSION=15-ea+33
# Fri, 24 Jul 2020 18:28:40 GMT
COPY dir:d2d12ac1efdebd3649782cfdcf4b9a26085a813f5cf403a1ea16348d252768f6 in C:\openjdk-15 
# Fri, 24 Jul 2020 18:29:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 24 Jul 2020 18:29:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17195adca743b283e9fdf01c1670d33e88c1b7f8ad0ff6a19afa11f90abbdaa`  
		Last Modified: Wed, 15 Jul 2020 02:46:29 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4978cbb8680255360d757c7d46e5a1c7c246047f93257964335958cd1b1307`  
		Last Modified: Wed, 15 Jul 2020 02:46:30 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0cf1f70e8582e4556e8be6e96025ad2d6e372cf6fdaaffb1cda64b76d8150f`  
		Last Modified: Fri, 24 Jul 2020 18:36:57 GMT  
		Size: 69.4 KB (69424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b2e2d468204c429e90685f0b28fc4a0bcb8c1b50ce01d726ca37b23d8a576`  
		Last Modified: Fri, 24 Jul 2020 18:36:54 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab82533a8d4c1fb568998245f98da31faf928183656891c1e05e6436056837a`  
		Last Modified: Fri, 24 Jul 2020 18:36:53 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9690ff9875d8ba5b4b6a075332a8a0df72e2eb9063a553221a3dee38cd0082e9`  
		Last Modified: Fri, 24 Jul 2020 18:37:17 GMT  
		Size: 191.4 MB (191359063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e78d326a104fbe9a41f3042a99634acf43998ae0641ce47ddef24603d5d7277`  
		Last Modified: Fri, 24 Jul 2020 18:36:54 GMT  
		Size: 3.5 MB (3498091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f258b33dc312a828554f1f6455a6a13a50808e42851f480b0a9ad6f6982ffc6`  
		Last Modified: Fri, 24 Jul 2020 18:36:54 GMT  
		Size: 910.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
