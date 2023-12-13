## `eclipse-temurin:11-jre-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:cebbc9193092669635d9ed4333425235df2e757d117f251bf9c054465dbd73e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:11-jre-nanoserver-1809` - windows version 10.0.17763.5206; amd64

```console
$ docker pull eclipse-temurin@sha256:2d6620faf7b308aa781c6654c30c368e44c3e41308fa341b0ef0be5518659b3d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.0 MB (148012871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9b6fb5f8ccf1bbf223939dbbce3400c0354d47d2902b60c1414149a2299590d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
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
# Wed, 13 Dec 2023 00:29:00 GMT
COPY dir:32725fa0f7edeee10e8937816f70b588636369ca6a0eb68560cc5c3b2b3f76d9 in C:\openjdk-11 
# Wed, 13 Dec 2023 00:29:10 GMT
RUN echo Verifying install ...     && echo java --version && java --version     && echo Complete.
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
	-	`sha256:edbbcb647886a555f9780d305afee6ff077b98a9d135daf95dfbddad4caae8b0`  
		Last Modified: Wed, 13 Dec 2023 06:38:42 GMT  
		Size: 43.3 MB (43348193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7ef5cd2d163816d6c654e3f25f22da3582118da971db2bf10e77938eb038dc`  
		Last Modified: Wed, 13 Dec 2023 06:38:35 GMT  
		Size: 81.6 KB (81552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
