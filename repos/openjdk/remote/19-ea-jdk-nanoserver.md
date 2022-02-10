## `openjdk:19-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:34160128040e064bc0ce1f0d218454225df32b00bed2e99cf1ae8ad37e4e7819
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:19-ea-jdk-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:83cde1858989e495b8898057932a26fa9606bb7c89155e9df6e3f48d90bf2313
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.6 MB (291647720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9b37817f32020df445543028c2154db7e211489d520bb6da9e0aeb4a0cb3004`
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
# Wed, 09 Feb 2022 18:45:47 GMT
ENV JAVA_VERSION=19-ea+8
# Wed, 09 Feb 2022 18:46:17 GMT
COPY dir:085c70939dba172f061bec7e04a177fe07855c76d2d86340a67635a03ecbe2d1 in C:\openjdk-19 
# Wed, 09 Feb 2022 18:46:30 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 09 Feb 2022 18:46:31 GMT
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
	-	`sha256:644af5af58d1fd1b43ecf86824eb5b1e60e3c13ff2f4adbd90a513ea4664ec67`  
		Last Modified: Wed, 09 Feb 2022 19:20:47 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b8b801bed0435aaa4ec7e69c18a0da21bd36e0d55a737025aba5b9e621ec9`  
		Last Modified: Wed, 09 Feb 2022 19:21:07 GMT  
		Size: 185.0 MB (184957559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8e988e1301c5bbd3ece5d83bd4ed6f5f5b32276934bb95110ca7b9d3a6dc5c`  
		Last Modified: Wed, 09 Feb 2022 19:20:48 GMT  
		Size: 3.5 MB (3518395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6408a0553b82b65782a2f0d3735ed28a6134fce5df861dc8bc9caa807f6d3cf`  
		Last Modified: Wed, 09 Feb 2022 19:20:47 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
