## `openjdk:19-ea-9-nanoserver`

```console
$ docker pull openjdk@sha256:c83ef634ccac4e503fe7ddf020408dbbc6434bfc96cc95c633535f074e5827f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:19-ea-9-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:8a6a18050d83c3a0853b73ec569e96213321ef48ba3e51d5ca267ee1cbf82ffc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.7 MB (291663930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:372159d5e02ecb40e3b578fcb35d84b6ec47427df1ec50ba5d0ccdd7c8e75831`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 18:45:33 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 09 Feb 2022 18:45:33 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 18:45:46 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 18:45:47 GMT
USER ContainerUser
# Fri, 11 Feb 2022 23:18:39 GMT
ENV JAVA_VERSION=19-ea+9
# Fri, 11 Feb 2022 23:19:12 GMT
COPY dir:1c95d8372c1ae9fb04d81e47db2840226b597af9d6eee6a36d313f6130148ad3 in C:\openjdk-19 
# Fri, 11 Feb 2022 23:19:27 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 11 Feb 2022 23:19:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5a7f567e84a5a148036156650a47ef7eec0187f17e880d3b475e51dacd70077b`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69acde47ea38ca917ac70bd099e8642e4d106e4d031254a5bd61c52e9e93a26`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a983d7a89070a62890b5312d217fb42c0a23a81f4b88020f86dd774b681bd5`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798ff236fae94b7a9651e0beb7fde720729c184b3d3150895ba4d507d0b4794b`  
		Last Modified: Wed, 09 Feb 2022 19:20:49 GMT  
		Size: 77.7 KB (77739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b819309b74b4730666b4d3b76627010d142d418aa74b8068c4e4af5d3d77b23`  
		Last Modified: Wed, 09 Feb 2022 19:20:47 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea35cd5de48e653efe137fe1fa61093448a1dc7cbf549fbdfe8204d30267849e`  
		Last Modified: Fri, 11 Feb 2022 23:40:49 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd02f90da55c2aa628d680cc05ce2229a2c0298966b01d900a561e36829ff758`  
		Last Modified: Fri, 11 Feb 2022 23:41:10 GMT  
		Size: 185.0 MB (184967759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86211f37391581397d88ae59e8cc6977c215828e79d0b08adbea87fd1686aa02`  
		Last Modified: Fri, 11 Feb 2022 23:40:51 GMT  
		Size: 3.5 MB (3524370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477875c0f5a3bb939c5703ee7a26706b967d648a355d7cbf2bc5d1fc1eb0abb`  
		Last Modified: Fri, 11 Feb 2022 23:40:49 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
