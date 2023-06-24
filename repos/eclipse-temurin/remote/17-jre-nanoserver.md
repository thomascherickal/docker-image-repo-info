## `eclipse-temurin:17-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:a77e823698fcdde892d796e5d5cd6521eb960c7cc529196475badc6c714eb8a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:df0ef35b4d10193024a23a0eccca923a1a203850fc9527ceffd6d082b86735e3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163528217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77ec1f1a71e1c864aaa7f8080ba462a5e1c0aaafd37534a4a1602047e6dffa50`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 24 Jun 2023 01:12:02 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Sat, 24 Jun 2023 01:12:15 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:3af5446ed014100cfd7e7bbd1077225338c5dc48543b19de514c0e33c4a07987`  
		Last Modified: Sat, 24 Jun 2023 01:36:36 GMT  
		Size: 43.3 MB (43328540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bab415e2f829b580f467b87e6933def60cf6c8525a426f6ac2265f42516ba`  
		Last Modified: Sat, 24 Jun 2023 01:36:27 GMT  
		Size: 72.3 KB (72324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:17-jre-nanoserver` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:6e846c6408f69bed89abfbe916d4a396fd426137b1ca31afb9a7b6f0101b15b2
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150837941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:530b3df41f512e026dcdfd11656ef15c065e944cace31057b5b01945c0f94995`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 24 Jun 2023 01:00:15 GMT
COPY dir:8912d07424b5206284ef3b7586d69c3f366b527bba3d6f334194ae58c2152641 in C:\openjdk-17 
# Sat, 24 Jun 2023 01:00:27 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:3a0e4ba7cec9c420a6b75eac35aab2944112067b107984da8179bd6f2aa6aa3d`  
		Last Modified: Sat, 24 Jun 2023 01:31:24 GMT  
		Size: 43.3 MB (43328726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a2d63d93453c74afa69a7b38014e9107b3fb30b04e4b93e8714d1d6677f298`  
		Last Modified: Sat, 24 Jun 2023 01:31:17 GMT  
		Size: 3.0 MB (3032403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
