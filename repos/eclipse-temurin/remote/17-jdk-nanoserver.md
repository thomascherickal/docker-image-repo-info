## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:fd9c82486fc3f568380e75074a986d09e16ab5388b109f048300d0f413a10c92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.350; amd64
	-	windows version 10.0.17763.2300; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:a9716df0b9fbd2341a5c91372729bb9481ac40ca28c84e5236aeea249ff5ac67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.2 MB (302219620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28aaf143a0aee3ea2c726c194c566097976712608e94bbea7dc08b860d839283`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:54:54 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 10 Nov 2021 17:54:55 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 10 Nov 2021 17:54:55 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:55:05 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:55:05 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:55:20 GMT
COPY dir:75727e79a870c9066772bd3811959a8f3c491ac4b54ae3b2c145d1638b6bc93f in C:\openjdk-17 
# Wed, 10 Nov 2021 17:55:33 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 Nov 2021 17:55:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d9ade421e04ec15d030759d534fa2954faca2f1fd01138dfc9f1e14d89d858`  
		Last Modified: Wed, 10 Nov 2021 18:59:15 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe357e35906ee226eb55c8d08ea46204af0769fc8583e518cc7231498ec0c9f`  
		Last Modified: Wed, 10 Nov 2021 18:59:15 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce5df4f7dd6b0da9f1608363f096e7fa7b2e1a1240d8e5bca265bfc314034bc`  
		Last Modified: Wed, 10 Nov 2021 18:59:15 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209ffa41ea3a0fce7bfed2f4d4e76e55b1f7fd28dcedee9025125799c73dc21e`  
		Last Modified: Wed, 10 Nov 2021 18:59:12 GMT  
		Size: 85.8 KB (85757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6435f1721cbb1db4b0ecabcf56a1fc29032c511d7e5b1acc1076d22e5c6415a`  
		Last Modified: Wed, 10 Nov 2021 18:59:12 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502ad2c6de06f69ff87a574a7e081aa3c61d063071da2a8a89e4417ab397208f`  
		Last Modified: Wed, 10 Nov 2021 18:59:31 GMT  
		Size: 184.9 MB (184948352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9321b9a2d2a3fc6447eec4cead964a0c255ef457c0e230462a482af02b8c8a93`  
		Last Modified: Wed, 10 Nov 2021 18:59:12 GMT  
		Size: 61.7 KB (61717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2964f5448020bbb0f0e599c46819b8deed682dac33a4ad76b98d4539c2a571`  
		Last Modified: Wed, 10 Nov 2021 18:59:13 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.2300; amd64

```console
$ docker pull eclipse-temurin@sha256:1a8af4af368ffad0f5f935fb9eaaeee508ef46170b8a2c122f9e7ac9e91d868c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.5 MB (291459241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954c44ee33146e1c3d9665c44903785f13cb452b64faae6307aabd0081d1df99`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 04 Nov 2021 00:06:50 GMT
RUN Apply image 1809-amd64
# Wed, 10 Nov 2021 17:13:20 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:48:30 GMT
ENV JAVA_VERSION=jdk-17.0.1+12
# Wed, 10 Nov 2021 17:48:30 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 10 Nov 2021 17:48:31 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:48:40 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:48:41 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:48:57 GMT
COPY dir:75727e79a870c9066772bd3811959a8f3c491ac4b54ae3b2c145d1638b6bc93f in C:\openjdk-17 
# Wed, 10 Nov 2021 17:49:10 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 Nov 2021 17:49:11 GMT
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
	-	`sha256:e575c8ac67cc054719119a20b1580ae57730dac36cfd352e46f944aeab938c5f`  
		Last Modified: Wed, 10 Nov 2021 18:52:49 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1d9705dfb694c80422b73df7c7a45bdca91316ed34954c1544835845b11e9c`  
		Last Modified: Wed, 10 Nov 2021 18:52:48 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bde24854f60eed18c08aa3f2e03e2bee1def318563dbf24f6508b3f8e178aeb`  
		Last Modified: Wed, 10 Nov 2021 18:52:48 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b104476a313be1839344cf9a1522bd494f20a8de3165dff0e9e20e0d74a9981`  
		Last Modified: Wed, 10 Nov 2021 18:52:46 GMT  
		Size: 70.5 KB (70523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fc726fe8dc2a1788510b52b4683f4be40d7d4016d64d5afa1f7f02a7a26407`  
		Last Modified: Wed, 10 Nov 2021 18:52:46 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6428eaf6fa6218043b5f336bfd70feaa91003252c0bd14461764056f39c1d68`  
		Last Modified: Wed, 10 Nov 2021 18:53:04 GMT  
		Size: 185.0 MB (184952172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5407de9e435c3a1426e402d766852a17a17ba7ad7ec0f12497613372f24579a`  
		Last Modified: Wed, 10 Nov 2021 18:52:47 GMT  
		Size: 3.6 MB (3646607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d96c18aef7ec222654e0ebd8259c3974c42aa80ed1e93bf5dd6d1779616e9`  
		Last Modified: Wed, 10 Nov 2021 18:52:46 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
