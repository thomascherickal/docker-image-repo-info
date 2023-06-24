## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:daad619a9615dab268e5004e600f8c6d1afc7f6b44d55c0afddb60137e8bac32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:e398b9d967f61c31360e2de63682608b29829e1b7354c0630fdec83624e0547d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.5 MB (297546975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ab3172d7136cae165b06a2d141fa06a022dc150a0a8362ff4cfd758dc614aa`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:40:33 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:41:51 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 00:48:59 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 00:49:00 GMT
ENV JAVA_HOME=C:\openjdk-11
# Sat, 24 Jun 2023 00:49:01 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 00:49:10 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 00:49:10 GMT
USER ContainerUser
# Sat, 24 Jun 2023 00:49:26 GMT
COPY dir:aa85dc89894032bdcf98e5da06633e8de4813537c791ddbe3fc8bdfa8596f8de in C:\openjdk-11 
# Sat, 24 Jun 2023 00:49:39 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 00:49:39 GMT
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
	-	`sha256:d6ab3e6e6dd66405d6519f123dde5332888aa883897c7f2310ec4cde998e2876`  
		Last Modified: Sat, 24 Jun 2023 01:27:25 GMT  
		Size: 1.1 KB (1074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eec62241a5ffda3ad10f0cedb4c6748d61fd258086785e7b88adc0bc020a9a3`  
		Last Modified: Sat, 24 Jun 2023 01:27:25 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b27c01f4bd625e6165da949fb411ae920a9034436ca8d816b4bb064c8e9b1e`  
		Last Modified: Sat, 24 Jun 2023 01:27:25 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a34d4368984cbad3ef8a584fb4056359ee05d0492fc6613a7efb8023755cd8f`  
		Last Modified: Sat, 24 Jun 2023 01:27:23 GMT  
		Size: 68.0 KB (68004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49c2148183a82fae049ad9e73a156e92cf5cf86b3f145eb5e1be3008c1db5d1`  
		Last Modified: Sat, 24 Jun 2023 01:27:23 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93ca24faf431ca864b8a64d05868f1d371c966dca9f3371d268246037e6aac4`  
		Last Modified: Sat, 24 Jun 2023 01:27:42 GMT  
		Size: 193.0 MB (192981920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffa10b83802955f4cb78d77785b262986aa3a1a4d588232d99dd0e93424eded`  
		Last Modified: Sat, 24 Jun 2023 01:27:23 GMT  
		Size: 89.8 KB (89808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b635b76f161ff0ab2df04a9760cf17c24265702347ba55b2a7ad0670b8eb58f8`  
		Last Modified: Sat, 24 Jun 2023 01:27:24 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
