## `openjdk:18-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:017d7aae7d8784649bf0aa3ce43bcb39c6c6687e839848c2b13ed261443d67df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:18-ea-jdk-nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:b20ea151857e1878988b1523673c1a3ca2b230429b503dbe049b925fcaa0521c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289512272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44468e04cbec58a492c05876820b27f40e84206848309ee2a7a0e7eaec7ead16`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 00:38:45 GMT
ENV JAVA_HOME=C:\openjdk-18
# Thu, 14 Oct 2021 00:38:45 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 00:38:59 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 00:38:59 GMT
USER ContainerUser
# Thu, 21 Oct 2021 23:20:28 GMT
ENV JAVA_VERSION=18-ea+20
# Thu, 21 Oct 2021 23:20:53 GMT
COPY dir:d6f9c5d9946fa63761bec751cc4fe7d46bf1d78ccb8a219d0b98159674502a4e in C:\openjdk-18 
# Thu, 21 Oct 2021 23:21:31 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 21 Oct 2021 23:21:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11210a1a14144795863cc9df7368535adbfcea9f756732c5757ce09ae1126ff9`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4f8f1bc44cf5deaf0e09239eb5f99652025d58114cc36025894b724e1e593`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528cd68420af607e2ba2867ba7f9e41b2412cc5fcd6ad946de4355966a18b56b`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 71.6 KB (71641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee7149c120a9a849ece2e9be315293f5b77a4443d8f1cc13b6d4745290851a9`  
		Last Modified: Sat, 16 Oct 2021 00:39:34 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41461d7058533022196f9af052d8b5f8b6c8e5432e994332e360d41a001e887`  
		Last Modified: Thu, 21 Oct 2021 23:43:37 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0371dd32abffbf50605f46c6bfe1fee5388154d631e3174a1b044c8cf66e0b`  
		Last Modified: Thu, 21 Oct 2021 23:43:58 GMT  
		Size: 183.2 MB (183240134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f95b1bdc3025435e1b820ede7d3c30896302d4dcbd6d44a2b52fc8631b536`  
		Last Modified: Thu, 21 Oct 2021 23:43:38 GMT  
		Size: 3.5 MB (3532268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d658a2df01df78d2208920e4521eb20467f74ff4e454d6eb37f496d68040cba4`  
		Last Modified: Thu, 21 Oct 2021 23:43:37 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
