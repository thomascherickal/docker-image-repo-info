## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:55c435613ce63d5bea48daefc7457bf512fc717478fe91a5741647b9d7d50daa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:d096f00d592b0f0bac91c32827b0457c3ea8cbab08a9d6137205fac692ea121e
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.7 MB (147726989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b8754f8f786fe895efb12abc43c7812489e25cc90b73ec483c3d5703efe4211`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Sat, 24 Jun 2023 00:52:17 GMT
COPY dir:b6e5aca1f3f361bc79d6ed078f0846fae24cf0b7748963379a92b2a6511b98d8 in C:\openjdk-11 
# Sat, 24 Jun 2023 00:52:27 GMT
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
	-	`sha256:00b1eb911488fc5db5919a3d2a6388900841901b7fe5b30f03fbfbb1af32a77d`  
		Last Modified: Sat, 24 Jun 2023 01:28:40 GMT  
		Size: 43.2 MB (43172551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734ab2991e5f20e16798bda7ff00f5bb41d79d9fb075d14c79a550a2d268a4b3`  
		Last Modified: Sat, 24 Jun 2023 01:28:32 GMT  
		Size: 80.2 KB (80224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
