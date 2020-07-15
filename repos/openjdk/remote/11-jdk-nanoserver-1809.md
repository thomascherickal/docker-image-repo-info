## `openjdk:11-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2ba37b547172484c9c6f644803788aa8c4caf6f2ed3cdf7ad828256545a93427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:11-jdk-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:a5547df8a7c5bc60a449e60e3c09fb7f8c65b71f0c9917483238fdd7859e1bfe
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291026770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1dd96a373fb53c09d571996a680c07a7df21067cae899a122f77435d6017ca0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:21:21 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 15 Jul 2020 02:21:22 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 02:21:33 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 02:21:34 GMT
USER ContainerUser
# Wed, 15 Jul 2020 02:21:35 GMT
ENV JAVA_VERSION=11.0.7
# Wed, 15 Jul 2020 02:22:29 GMT
COPY dir:d90d60e1c0505496926373a51cab7b6b2c4fc0bb30d14b79fe3ef70ac0ba6a6a in C:\openjdk-11 
# Wed, 15 Jul 2020 02:22:46 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 15 Jul 2020 02:22:46 GMT
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
	-	`sha256:1edf2cf232929022745a17a752c11091206fd6804fbcd0deb0cf94f65d838e43`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34289060bcecad92a4781d988ddd844d829452e51a1c73c3f2608a0a6085c77`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 909.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78522c618af5554ffd3adf8623d7933e1792428e86ad573127cee6fdc3a590d`  
		Last Modified: Wed, 15 Jul 2020 02:51:37 GMT  
		Size: 64.2 KB (64206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5608ac22c3f2ef90c8c5bc20a0fe2c584d51c075fe6bf2a5b7509df4c32d755d`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5471947ff5dafa77f1d05926afd2d7caaa25c826f05f5cf8a6dc597d83777`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02772a2467ac239c8099db3f824fa2e8d8ed30c902e08e2a5cd9232191a683b`  
		Last Modified: Wed, 15 Jul 2020 02:51:55 GMT  
		Size: 190.0 MB (189976050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8044b9d5b7caa1df340a03620fdc01eb4adc511b5b6672a17c4ef6c5770262e`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 85.6 KB (85565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f094efbae377ecaa34fac299d66547e3284222735253b31d4c10a6919f58f3`  
		Last Modified: Wed, 15 Jul 2020 02:51:35 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
