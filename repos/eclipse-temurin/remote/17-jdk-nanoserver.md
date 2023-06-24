## `eclipse-temurin:17-jdk-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:e1595e3abc81cf5e10195de8b6c939ff0e3eddd4d5bc5633bd483c8c3652f1cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:bc20674591bbc986dcbd7100567ebfb9197c1ab17d0aa84a5417e7fb8a299fa5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305738975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1153fef93e5db52dcb1e512588532f03caeb0c29db1c33608b466b8bbd02e20a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:11:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Sat, 24 Jun 2023 01:11:03 GMT
ENV JAVA_HOME=C:\openjdk-17
# Sat, 24 Jun 2023 01:11:04 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:11:17 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:11:17 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:11:33 GMT
COPY dir:124ac1113930ce4049263b0be6b87edbaf53b403e9545bc9faa31b4eed61cbf5 in C:\openjdk-17 
# Sat, 24 Jun 2023 01:11:48 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 01:11:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11441d3b24271b5fa26c70c21bd288bae051f6076d292e108c508d7587457045`  
		Last Modified: Sat, 24 Jun 2023 01:35:59 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db08e6136622be31e49ed7679b0a275107dd072ab770ab8bb01afe3c990481dd`  
		Last Modified: Sat, 24 Jun 2023 01:35:59 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398bb987a0ed27e9689a2c403983a0973f3b438020adf79def2c31f5d9f35187`  
		Last Modified: Sat, 24 Jun 2023 01:35:59 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a136d456d605b4dc5c5e839575228536c876bf16177875308fef070e754cfc2`  
		Last Modified: Sat, 24 Jun 2023 01:35:57 GMT  
		Size: 93.3 KB (93252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618cb8619c31ae7931033eff2003cea36652c8b6a76d21cd04be8a66238e5d77`  
		Last Modified: Sat, 24 Jun 2023 01:35:57 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252b7e14542311a65b3916fc6b15857134b85d57d551c8b034f37fe58c837e88`  
		Last Modified: Sat, 24 Jun 2023 01:36:15 GMT  
		Size: 185.5 MB (185538202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47eed90eb881cdce04814a0cfc62005eef1d74f7421cb4702cd00d61f0b781d`  
		Last Modified: Sat, 24 Jun 2023 01:35:57 GMT  
		Size: 72.2 KB (72250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159e42ba009873a4bb77f52b498205abbd50232272da9626a1b4833a6e268f53`  
		Last Modified: Sat, 24 Jun 2023 01:35:57 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jdk-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:c3ce4fafe27637cfe9ed2c716df7b57260001feedfc4acd129055a8e8e3b0ead
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.7 MB (293674569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ac4e19757bef03cb4201b900a19bca5f0e16e6644039c67474e481c8a60a97`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 00:56:03 GMT
ENV JAVA_VERSION=jdk-17.0.7+7
# Sat, 24 Jun 2023 00:56:03 GMT
ENV JAVA_HOME=C:\openjdk-17
# Sat, 24 Jun 2023 00:56:04 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 00:56:13 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 00:56:14 GMT
USER ContainerUser
# Sat, 24 Jun 2023 00:56:30 GMT
COPY dir:124ac1113930ce4049263b0be6b87edbaf53b403e9545bc9faa31b4eed61cbf5 in C:\openjdk-17 
# Sat, 24 Jun 2023 00:56:46 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 00:56:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:09087aac643f57e5e24f95fe0a1c8519d0f93dfcf4500263516c0f3874290109`  
		Last Modified: Fri, 23 Jun 2023 02:23:11 GMT  
		Size: 104.4 MB (104400893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09be2e47b3dff420361e93d34eaadedcfd9549c9be5bd77936370792babf874`  
		Last Modified: Sat, 24 Jun 2023 01:24:43 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a031e3cdb2804bf2b91fc71c4c6f212b913f05ba7b374524037b334b7fda6b`  
		Last Modified: Sat, 24 Jun 2023 01:30:09 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d929788d34c7bc5ad9ca602979f2cf36dda66a189b1be4f606dfd86ba5abdbfc`  
		Last Modified: Sat, 24 Jun 2023 01:30:10 GMT  
		Size: 1.1 KB (1078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5957c883ab0557961af39447c869d7c70d9653cd6f8c4cab25f9f35e5a090c97`  
		Last Modified: Sat, 24 Jun 2023 01:30:09 GMT  
		Size: 1.1 KB (1071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b13806df0dcc551ac5a8647513a3f108ea22791870c8ee57c78dce4ae76e63`  
		Last Modified: Sat, 24 Jun 2023 01:30:07 GMT  
		Size: 70.5 KB (70467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3fb0ff857940488eeaab46badeb18556da0beea6f28e4e3ccd90974dd69d93`  
		Last Modified: Sat, 24 Jun 2023 01:30:07 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97af53a1d5b5386708e725e05b70b3e26dd188d4209776aa226ee1e7b63081a6`  
		Last Modified: Sat, 24 Jun 2023 01:30:26 GMT  
		Size: 185.5 MB (185535613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b73a802063552be88529c1ae1de16b3ec8d6047dd1b44401e33863cff3c197`  
		Last Modified: Sat, 24 Jun 2023 01:30:08 GMT  
		Size: 3.7 MB (3661077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e5bcd023cf3af8fa69a72e492b845ef772e373622a1062afdc44f35ddcc70d`  
		Last Modified: Sat, 24 Jun 2023 01:30:07 GMT  
		Size: 1.1 KB (1067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
