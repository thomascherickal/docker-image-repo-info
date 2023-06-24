## `eclipse-temurin:17-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:14d3a815b7450cf47aac7f1e8bcb14db10c23f75395c0fc71f234ccc4234f6f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:17-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

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
