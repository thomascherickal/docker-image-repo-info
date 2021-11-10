## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:7a5a57d602697ccd915a1b2cbbd3539019461c06407e186abf2470ab19637c69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.350; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.350; amd64

```console
$ docker pull eclipse-temurin@sha256:6cd074e8fb23d7bf25c60c6455c0c3175d4b5f950e0b8429caf6248b7778ef67
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.2 MB (309194840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf328bd164ec7983a53735c5007402441aac03704b959971582c9c9249df60c2`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 03 Nov 2021 08:13:55 GMT
RUN Apply image ltsc2022-amd64
# Wed, 10 Nov 2021 17:52:19 GMT
SHELL [cmd /s /c]
# Wed, 10 Nov 2021 17:53:35 GMT
ENV JAVA_VERSION=jdk-11.0.13+8
# Wed, 10 Nov 2021 17:53:35 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 10 Nov 2021 17:53:36 GMT
USER ContainerAdministrator
# Wed, 10 Nov 2021 17:53:45 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 10 Nov 2021 17:53:46 GMT
USER ContainerUser
# Wed, 10 Nov 2021 17:54:02 GMT
COPY dir:7549fd743977f7762910679960e9adfeab116385590a40bc0f1570100fce1af1 in C:\openjdk-11 
# Wed, 10 Nov 2021 17:54:14 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 10 Nov 2021 17:54:15 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:83b9a19f898e6e25b6ee7e787da89582a8528b2defb5682f45364d04b35a278d`  
		Size: 117.1 MB (117116823 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:38ddab3f86968a251743624cdf77bd5cbcafea760b8951be49f84bc3bc5b82a6`  
		Last Modified: Wed, 10 Nov 2021 18:53:58 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e60a18aefb5c5bb8955067d23b9a2f7d1157a88831ce6b2071cec8e581f077`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab70470578cfb024d7d073a90446e09fa7f464faf9d307a6600607d8c10471b5`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a719fea5e976f3229d956e7e3371e962995af4e615fa7a7badeac24443be7`  
		Last Modified: Wed, 10 Nov 2021 18:54:37 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796f2ca8a54d4f8b5df8581be27e1229d8ab11142cc1a1c26e47c15f373122d`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 83.5 KB (83528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5bee5015e8ba92e3c8630de1842c7e17dec954ce3d3ce5fc2a769042c2792f`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c4289311e6c6641146315a89be0c0d328190e05516e677e5f6da01b958b429`  
		Last Modified: Wed, 10 Nov 2021 18:58:03 GMT  
		Size: 191.9 MB (191925653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4197ae443fd60191eed8d98306aaca07f24a78ecef4edf656794ed188f88c3f9`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 61.9 KB (61937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cfba1fadeaafa5c1a30004d1e94b95a9217c4fa0f7039dcd22b88870f81be9c`  
		Last Modified: Wed, 10 Nov 2021 18:54:35 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
