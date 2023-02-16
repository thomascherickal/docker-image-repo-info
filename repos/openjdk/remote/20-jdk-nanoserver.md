## `openjdk:20-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:a06730fdfadca870ff66cad2ebe2e5a56a4a02232e1cb3a566bad4f964bb3bda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `openjdk:20-jdk-nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull openjdk@sha256:a16d5014acb2cd9d37fb9bf10c7221a28c8b1b9ee030784fe1d03f988c48577d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.6 MB (303632323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b82b8489d51c92ba8971fa9aed64544f098ccbccba5634e370fb29158b4a411`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Wed, 15 Feb 2023 22:46:15 GMT
SHELL [cmd /s /c]
# Thu, 16 Feb 2023 02:25:54 GMT
ENV JAVA_HOME=C:\openjdk-20
# Thu, 16 Feb 2023 02:25:55 GMT
USER ContainerAdministrator
# Thu, 16 Feb 2023 02:26:07 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 16 Feb 2023 02:26:08 GMT
USER ContainerUser
# Thu, 16 Feb 2023 02:26:09 GMT
ENV JAVA_VERSION=20
# Thu, 16 Feb 2023 02:26:25 GMT
COPY dir:993cb869459fba742419cffbcf553ece0591a50d69cbcdfd0aea8e998cf9d7ec in C:\openjdk-20 
# Thu, 16 Feb 2023 02:26:44 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 16 Feb 2023 02:26:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185f49bd9e9c2d18b1dcf8f1f67123b4146383e07a158cb4623d96fb2d18c05`  
		Last Modified: Thu, 16 Feb 2023 02:29:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042953a596eb2aefd489398e31c7f1ec6ef46f488b30ff8fb0ccf507ea79793f`  
		Last Modified: Thu, 16 Feb 2023 02:31:07 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d3b56749fab7e03c419bb3662f0819810e094479b606e2ad54e31fa6af491d`  
		Last Modified: Thu, 16 Feb 2023 02:31:07 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7debab9bbd192fe6092151b00a5e2c660f24dfa88f25a53192b9e8d464a90eb1`  
		Last Modified: Thu, 16 Feb 2023 02:31:07 GMT  
		Size: 70.1 KB (70065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9a8c9daac90543d5739d2d8d435bb989e7f7c2f385fa79674ddef1acfa98c2`  
		Last Modified: Thu, 16 Feb 2023 02:31:05 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01d186fecb44d6e06cc75e53e02d07469afe6b6043de0de3628a709187cc944`  
		Last Modified: Thu, 16 Feb 2023 02:31:05 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcf454ef939475f1d01f7369b53f21941705746a5e262aaa649c1ef468f68d5`  
		Last Modified: Thu, 16 Feb 2023 02:31:25 GMT  
		Size: 193.1 MB (193082159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9978ddc79953e8a5eb1721355cea4fb002394def4764ce452db3cd70a2a32a`  
		Last Modified: Thu, 16 Feb 2023 02:31:05 GMT  
		Size: 3.8 MB (3798208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff3f268146e1dce4016ee9dab1f502827b0902302cc766739d5f5263b745f7d`  
		Last Modified: Thu, 16 Feb 2023 02:31:05 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
