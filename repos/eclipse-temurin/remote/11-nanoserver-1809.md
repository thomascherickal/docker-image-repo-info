## `eclipse-temurin:11-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:d5b51b7809c8251aad752edaee3dd5a7ea469973e6260d6a2f271f6f72abed66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:11-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:cb27618b949043569d795ea0c5b7329a73eea4c87ccccf924f06486c25b499b8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.6 MB (298642329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb04a5b7b472a1d31f7371fd4181c1f19f6cbf4a8a3a7b5987ab70dc239a4b9`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Dec 2023 10:54:04 GMT
RUN Apply image 10.0.17763.5206
# Wed, 13 Dec 2023 00:14:36 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:24:13 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:24:14 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Dec 2023 00:24:14 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:24:23 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:24:24 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:24:37 GMT
COPY dir:3378004dd1c559f9d7d6f4bacd149386aa6ab741f7dba391fbd8a10b1a80b205 in C:\openjdk-11 
# Wed, 13 Dec 2023 00:24:49 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 13 Dec 2023 00:24:50 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:424f13a93a185a5defe848e7d270655e05233555f51328c0af24b9e70677d037`  
		Last Modified: Tue, 12 Dec 2023 20:02:40 GMT  
		Size: 104.5 MB (104510104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d6d8b15609381c4993ee309513fbc3fc2b2b34fb28651d28f25e975b2fe403`  
		Last Modified: Wed, 13 Dec 2023 02:22:34 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544521c66e8fe83593187511572849c3f27498c9935a8886186c271d562f75b1`  
		Last Modified: Wed, 13 Dec 2023 06:37:31 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bc53ad22815f7a15ad3b499ea7d8ce6893ebc7f401749bcaf079f27f1a0da`  
		Last Modified: Wed, 13 Dec 2023 06:37:30 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8f275a53a0971e8bc69064ed182f03c15af64ba8d139c0a948337fdba1a70d`  
		Last Modified: Wed, 13 Dec 2023 06:37:30 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c829a98cbad6dc1fa2690e75b2df1d37f21611d11b8af3d751e21863f31253bd`  
		Last Modified: Wed, 13 Dec 2023 06:37:29 GMT  
		Size: 67.7 KB (67695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b7905d3900fae7e9dfee93578a75455e6fe5106d119237550b0860d6cb279d`  
		Last Modified: Wed, 13 Dec 2023 06:37:28 GMT  
		Size: 1.1 KB (1066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a60dfa59e1661a4080ca6ea42366230030fb0bc29270c07a57ad0200205ddc`  
		Last Modified: Wed, 13 Dec 2023 06:37:45 GMT  
		Size: 194.0 MB (193968225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bec246e97a2ab430c05248120788c4e7f12ba342968c05c732140c8885d23e6`  
		Last Modified: Wed, 13 Dec 2023 06:37:28 GMT  
		Size: 89.8 KB (89819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17c462215b4b9c7552002eff6e01a7b43e3d7e0f49ef3675d1bb8701eeba061`  
		Last Modified: Wed, 13 Dec 2023 06:37:29 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
