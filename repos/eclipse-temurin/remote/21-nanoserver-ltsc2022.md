## `eclipse-temurin:21-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:2a0ef1ba407b26f2038ba2f9a4cb8f4bb375c3e9eb276145418c93d6c598c819
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:21-nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:92d006af97f8ac226b006715eabf2e8fd651f191f3c1326290cff6407463d425
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321897118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e050044cd37bd39546673a9bcf38fd683be8c505b52670d94933f3ced05de0bd`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:53:08 GMT
ENV JAVA_VERSION=jdk-21.0.1+12
# Wed, 13 Dec 2023 00:53:09 GMT
ENV JAVA_HOME=C:\openjdk-21
# Wed, 13 Dec 2023 00:53:09 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:53:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:53:19 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:53:33 GMT
COPY dir:fd62014fea6b5cd8b6f3d34ff8f9c5e95aa0ce969b7fd9201e979e77a3abe050 in C:\openjdk-21 
# Wed, 13 Dec 2023 00:53:46 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Dec 2023 00:53:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:075332bb10f7fc70c56f7c073dd753e05cacbc93a38c181c5576739a29f8a7e1`  
		Last Modified: Tue, 12 Dec 2023 21:35:16 GMT  
		Size: 120.8 MB (120757041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e420e231f6e0404269e9ff487f0ffc079de3deb8c08e9ff31ccb5fda1d1a44ec`  
		Last Modified: Wed, 13 Dec 2023 06:44:18 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfc63bbd0c867ec621202574726e4764200ae89abbef9538a2fa69372f25d21`  
		Last Modified: Wed, 13 Dec 2023 06:46:34 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3221e6013cbc3d0b893cba81d512da4a2a562ebe1feb9af2997d6212f10fba0`  
		Last Modified: Wed, 13 Dec 2023 06:46:34 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602034c63b5155ca9580d2fb35236909c25aa2d5cd6aad6d277661de341dd3d2`  
		Last Modified: Wed, 13 Dec 2023 06:46:34 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a25fbd1e9c4007ef33f3eb74b562f0631c31c4843a81c0b60f78b65ddb0ad1a`  
		Last Modified: Wed, 13 Dec 2023 06:46:32 GMT  
		Size: 77.5 KB (77491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352d0bd98b3ac5fbffbdc76adf4b2c8ef25e0f6a35e01bc85a983c2164f22f4c`  
		Last Modified: Wed, 13 Dec 2023 06:46:32 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc38cd9571881466da5aed927db8fdf4ace1e23a314f189e8d92762fe37ff7c`  
		Last Modified: Wed, 13 Dec 2023 06:46:53 GMT  
		Size: 201.0 MB (200994587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07396fcea2048b9ec4a71a74cace26288d35a0f7d1d164f47e9d8fb29b491928`  
		Last Modified: Wed, 13 Dec 2023 06:46:33 GMT  
		Size: 61.0 KB (61032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee12f84147f4faa2fe4279cc3c566614736c7222fd17ca0f923f2ff2f39cd0a`  
		Last Modified: Wed, 13 Dec 2023 06:46:32 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
