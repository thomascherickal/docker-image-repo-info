## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c9dbdacdc2c1b3539ca30e7d69a0e54a5218fd34a86b27c499b5d4e482de10a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:d1f8b9f7ca272613e18490578da992bd5c4f30246de487fc172fdabe82f46cd8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141871294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b515a4d2b63fe0a1cae28f8b67864c6fbb91464c79c3d4334766bd2941e73509`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 19:02:37 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 09 Feb 2022 19:02:38 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 19:02:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 19:02:48 GMT
USER ContainerUser
# Wed, 09 Feb 2022 19:02:48 GMT
ENV JAVA_VERSION=11.0.14
# Wed, 09 Feb 2022 19:06:08 GMT
COPY dir:cfebfad0723a0ff7cb715c8613c7ff95f5bc09dd8224aed2718d72001e95ccca in C:\openjdk-11 
# Wed, 09 Feb 2022 19:06:23 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5a7f567e84a5a148036156650a47ef7eec0187f17e880d3b475e51dacd70077b`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac0bf48a54e2421f92f124b47d38ee9ad764043cc5f5cb52e8f8ba04f00ce99`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b623100c5e8a6de92e548ce8bc6390263e442d776c8437eccc5827c051c65826`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa70386997aa574dc9d8458d26c8e3871a3c8389b44b3b39c60ecf4a08278b5`  
		Last Modified: Wed, 09 Feb 2022 19:30:16 GMT  
		Size: 70.6 KB (70555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6524283bfbd3d6b592d22322ad58960ceaa05bd51127df706da1032f4f9d0188`  
		Last Modified: Wed, 09 Feb 2022 19:30:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c075298312d39592e95515f2a9f7dc9dcff074b16630436c578fc8ea2b8e3b`  
		Last Modified: Wed, 09 Feb 2022 19:30:14 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d703a215d8b45ea8172a0cd9cc03474914ef202f97154f7bdccf7e0a4db89f4e`  
		Last Modified: Wed, 09 Feb 2022 19:32:12 GMT  
		Size: 38.6 MB (38642578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5166f88fc6a67d503f667bcd3093a758ff552665c1f4b9733e945c1e0631e8`  
		Last Modified: Wed, 09 Feb 2022 19:32:05 GMT  
		Size: 65.3 KB (65254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
