## `openjdk:14-nanoserver`

```console
$ docker pull openjdk@sha256:7cc11e48710b6a774e9e384fb1fa6eb89cc4a35712a580295de4b00730ff06c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.914; amd64

### `openjdk:14-nanoserver` - windows version 10.0.17763.914; amd64

```console
$ docker pull openjdk@sha256:f709afdcd7439c75184bbe06008ccc9b13447483efc9e933996b0ebf0577e12b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.6 MB (297562194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a778f4c73c8bf947b009f7599c6511d0accfaac5d468ef5c714d4f1c6ad08e09`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 28 Nov 2019 13:16:41 GMT
RUN Apply image 1809-amd64
# Wed, 11 Dec 2019 18:49:48 GMT
SHELL [cmd /s /c]
# Wed, 11 Dec 2019 18:49:50 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 11 Dec 2019 18:49:51 GMT
USER ContainerAdministrator
# Wed, 11 Dec 2019 18:50:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Dec 2019 18:50:07 GMT
USER ContainerUser
# Tue, 17 Dec 2019 00:27:48 GMT
ENV JAVA_VERSION=14-ea+27
# Tue, 17 Dec 2019 00:28:48 GMT
COPY dir:869b653d115c539b6451d7c05755ce06493f1e03843ce2448ed03abad9c24bae in C:\openjdk-14 
# Tue, 17 Dec 2019 00:29:15 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 17 Dec 2019 00:29:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1951f408509ba9ddcf240ef5d838c72c5596f97a05b063446508f2ba15d510f2`  
		Size: 101.1 MB (101106116 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:163d55b77f49371136083ba8066ddbec4afad6e1f4fbba77fa4ffebc99a8098a`  
		Last Modified: Wed, 11 Dec 2019 20:01:21 GMT  
		Size: 945.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9326e4caa8f459874d77c281820948a0fa2e558568f484250684f714e368c0bc`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 953.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07bbc07ec7d9f59279b56946327222e61b8d576bc34eb8b70be4aa88b484d87`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c25567424a9bb0685aa9d0cc78a53b800a3447fff914466146890e6bf40dcdd`  
		Last Modified: Wed, 11 Dec 2019 20:01:19 GMT  
		Size: 63.9 KB (63920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6607ef629cd6ba3de9b2b3f57cdc6172ca483c4f285428321d4b04ce9b321db8`  
		Last Modified: Wed, 11 Dec 2019 20:01:16 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ab50442d6ae29ed9f7b7b0be19d46955fd381f0e508b0b308e909a3dbf1d3f`  
		Last Modified: Tue, 17 Dec 2019 00:36:33 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d973940196be4d25924c4ce3c77c15aa50b03239c7d8fdaea1961b2a617ea5c`  
		Last Modified: Tue, 17 Dec 2019 00:36:55 GMT  
		Size: 192.9 MB (192917305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:246566f74bc978a47889ba3ac2aeea90714c29663bbb1dec82482a4d7523fd88`  
		Last Modified: Tue, 17 Dec 2019 00:36:34 GMT  
		Size: 3.5 MB (3469214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e058f898ab2c75bcc7c57752ae3283edf531a8b3cc01dcbddd5bca629e67a961`  
		Last Modified: Tue, 17 Dec 2019 00:36:33 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
