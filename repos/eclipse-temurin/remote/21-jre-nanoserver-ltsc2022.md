## `eclipse-temurin:21-jre-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:697bff651d6ecb28f4622ec879dddacf4aae4ede0abae20d7219339b494a8b93
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.2159; amd64

### `eclipse-temurin:21-jre-nanoserver-ltsc2022` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:1f35bc1fc2865975e05ad6ddd6883a002997281b15308d1aa1a09002c0a1b8fb
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169590972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f343365e30f94c69f7f3eefdf981c16220f13141053081f581702479faa970ad`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Dec 2023 00:53:59 GMT
COPY dir:a5a397b00294543a7015e10bed54514e1c5f8af5ed3eff5933ba2b604ae103c1 in C:\openjdk-21 
# Wed, 13 Dec 2023 00:54:12 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:695aeee922f69e809502df476ad2c333bc19123fb0ff58ac3b41c0b20165ed69`  
		Last Modified: Wed, 13 Dec 2023 06:47:16 GMT  
		Size: 48.7 MB (48689578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd15f867d4aa4ffb9555c465f3213ce8c281f5abeb616df9c1f958f335312e1f`  
		Last Modified: Wed, 13 Dec 2023 06:47:05 GMT  
		Size: 61.0 KB (61043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
