## `eclipse-temurin:11-jre-nanoserver`

```console
$ docker pull eclipse-temurin@sha256:e39bb281063a13f24d0a95f97784f0443bc7551370a174200f47651a00fb8946
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.2159; amd64
	-	windows version 10.0.17763.5206; amd64

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.20348.2159; amd64

```console
$ docker pull eclipse-temurin@sha256:cb28242b613e49d1202ca599319a329424909a4640353b14fc560d6f2b63d8ad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164252280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8f5cabda5aba9c55e6c7323bc82684101f20256108608c2b2babefffc07b60e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 02 Dec 2023 12:14:23 GMT
RUN Apply image 10.0.20348.2159
# Wed, 13 Dec 2023 00:49:12 GMT
SHELL [cmd /s /c]
# Wed, 13 Dec 2023 00:50:41 GMT
ENV JAVA_VERSION=jdk-11.0.21+9
# Wed, 13 Dec 2023 00:50:42 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Dec 2023 00:50:43 GMT
USER ContainerAdministrator
# Wed, 13 Dec 2023 00:50:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 13 Dec 2023 00:50:53 GMT
USER ContainerUser
# Wed, 13 Dec 2023 00:51:33 GMT
COPY dir:32725fa0f7edeee10e8937816f70b588636369ca6a0eb68560cc5c3b2b3f76d9 in C:\openjdk-11 
# Wed, 13 Dec 2023 00:51:45 GMT
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
	-	`sha256:8364739f74c962f7fbf4b7ff394af465565732796c10eb9d055cf4faebd86532`  
		Last Modified: Wed, 13 Dec 2023 06:44:58 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2983a48f082e3e4ae942091789823a5340dbc4d5544cb9a048f5a301e304ff`  
		Last Modified: Wed, 13 Dec 2023 06:44:58 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf30174846575b4b8e781cf38356cf69d5f37247f4c7cde8dc4dee9db738228`  
		Last Modified: Wed, 13 Dec 2023 06:44:58 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd213cbb4583ab87435025b5b9793c6f0e19e62ef915d6872c322a9ffa53ec8e`  
		Last Modified: Wed, 13 Dec 2023 06:44:56 GMT  
		Size: 77.4 KB (77361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d330cd98fdc8774dff6afcb6b7667ccca35038c0e3f25d8eff3a29d6c19e15dd`  
		Last Modified: Wed, 13 Dec 2023 06:44:56 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9f134a37efe58ce9ff8e8d68f9adb742f9417d1bab0ae68f80bd229d5f82b9`  
		Last Modified: Wed, 13 Dec 2023 06:45:37 GMT  
		Size: 43.4 MB (43351016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28e4ab223a15447c7136e6088e9d9207ba13840b9073932d004a2f391a85547`  
		Last Modified: Wed, 13 Dec 2023 06:45:29 GMT  
		Size: 61.1 KB (61102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-temurin:11-jre-nanoserver` - windows version 10.0.17763.5206; amd64

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
