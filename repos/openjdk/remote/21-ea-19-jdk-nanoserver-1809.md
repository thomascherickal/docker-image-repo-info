## `openjdk:21-ea-19-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2a40d9bada54f92904640c845e1eec2d48c9b21b925a7f7181e5b044b733a569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `openjdk:21-ea-19-jdk-nanoserver-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull openjdk@sha256:4a1699a115d5de049884ac850132bbf44d00d41b4c57b78fb6ce4dac604c5964
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.9 MB (306887051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc93df612eceddaeb8caae8a0496358af0cddd9e3a277b728f9662b9cd9d025`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 05 Apr 2023 00:14:49 GMT
RUN Apply image 10.0.17763.4252
# Tue, 11 Apr 2023 23:45:41 GMT
SHELL [cmd /s /c]
# Tue, 11 Apr 2023 23:45:42 GMT
ENV JAVA_HOME=C:\openjdk-21
# Tue, 11 Apr 2023 23:45:43 GMT
USER ContainerAdministrator
# Tue, 11 Apr 2023 23:45:56 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Tue, 11 Apr 2023 23:45:57 GMT
USER ContainerUser
# Fri, 21 Apr 2023 19:17:57 GMT
ENV JAVA_VERSION=21-ea+19
# Fri, 21 Apr 2023 19:18:11 GMT
COPY dir:a023104923f715c98e4b0a844e0b07dc0efa8898c39003a9fc27fd4e7eb42dc1 in C:\openjdk-21 
# Fri, 21 Apr 2023 19:18:23 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 21 Apr 2023 19:18:24 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:af799fb2ff133c89311c6a42d34b8cb6c9b11d775f52e04ab08389d05e64ed1c`  
		Last Modified: Wed, 12 Apr 2023 00:53:10 GMT  
		Size: 106.8 MB (106788951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1db438f20b81fe0c031e4e3eee58d278fba7258d01057ff18964cccf70d41c`  
		Last Modified: Wed, 12 Apr 2023 00:52:38 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959014ae4c354475658573dc2e10e98575d191deef98e1f23bf7cb9f4768408f`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b662327c70093bac13b7d07354fdbcd6967cbc13aaac870ca2e077fafefceb8`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9446ad09d009884e8a1db2085ef50cd6467dc3270eca7bac27fca70698013943`  
		Last Modified: Wed, 12 Apr 2023 00:52:37 GMT  
		Size: 68.0 KB (68014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1335b1a9f9197626e9424d9d24737142c9d98659cc7f5510ca10378488d00b51`  
		Last Modified: Wed, 12 Apr 2023 00:52:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c20ede39f2ea7c48d2fde2d30308b89d10d91d86f20f7726113fb23c5b4574`  
		Last Modified: Fri, 21 Apr 2023 19:20:20 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ccd683dbc7b49342fb3b6e3e19d9ff03c4498d7acdd1674e6c83eafd4c1ba9`  
		Last Modified: Fri, 21 Apr 2023 19:20:38 GMT  
		Size: 196.2 MB (196247798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca3b413f7f53f91610201590a4d64e75bd762d95169f688830bd4450e02e2e`  
		Last Modified: Fri, 21 Apr 2023 19:20:21 GMT  
		Size: 3.8 MB (3775377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85c154cb449941fa6f559f8478f7ce57176cbfaf4f645c2643a65b7facdb055`  
		Last Modified: Fri, 21 Apr 2023 19:20:20 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
