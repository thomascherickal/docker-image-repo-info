## `openjdk:15-nanoserver-1809`

```console
$ docker pull openjdk@sha256:698d225cd904f5895bc9ac6527d2d8a38c74aee1bfac69e04a8cb1cf195c8dd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1098; amd64

### `openjdk:15-nanoserver-1809` - windows version 10.0.17763.1098; amd64

```console
$ docker pull openjdk@sha256:a3a6066b7a91c68591c4ff5594a0152c38ecb4311f156854580f44c531a162cb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.6 MB (296585253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660b1a6d4957654baa1b731aa4a48488fa2a6a686ac6e82fb6845c4cc6012d03`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 04 Mar 2020 13:28:48 GMT
RUN Apply image 1809-amd64
# Wed, 11 Mar 2020 14:56:25 GMT
SHELL [cmd /s /c]
# Wed, 11 Mar 2020 14:56:27 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 11 Mar 2020 14:56:28 GMT
USER ContainerAdministrator
# Wed, 11 Mar 2020 14:56:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Mar 2020 14:56:55 GMT
USER ContainerUser
# Fri, 10 Apr 2020 01:20:19 GMT
ENV JAVA_VERSION=15-ea+18
# Fri, 10 Apr 2020 01:20:56 GMT
COPY dir:4b0099682e8b4a04796ff18349ecd4655059bff1caaf3119e2b54efe2598d1ef in C:\openjdk-15 
# Fri, 10 Apr 2020 01:21:19 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 10 Apr 2020 01:21:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e709836e4dce2fa52689be79fedc1e3d040ba47ec2da2fc3b23f33fc6944b50`  
		Size: 101.1 MB (101050245 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a66be005a5120fc8bbc31290c77aa0e6580d02bc61948ef0602bf09a6ab61ba`  
		Last Modified: Wed, 11 Mar 2020 15:26:11 GMT  
		Size: 933.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa222a675c58ae4e16af815d117d614899889b99615416d258fea25600f704cc`  
		Last Modified: Wed, 11 Mar 2020 15:26:08 GMT  
		Size: 931.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca058e8ce192a6fd627d0c85ec3d6b2843d8adc7b0a24db65d4460a1388d514`  
		Last Modified: Wed, 11 Mar 2020 15:26:08 GMT  
		Size: 934.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adfe4646dd92a1ea69c4f00cecd622a93c1467830cd992635a0ba3bc689db93`  
		Last Modified: Wed, 11 Mar 2020 15:26:08 GMT  
		Size: 67.2 KB (67155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348a60ea8643e6600613c06514ce34cb7bf596bd992df4b5f09a9e3b9226f76`  
		Last Modified: Wed, 11 Mar 2020 15:26:04 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6bbb389542594439fc8c6c7c8df8f636cd436c9ef77ba41fa696b58511aa1b`  
		Last Modified: Fri, 10 Apr 2020 01:25:55 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5e4c2098dd4b58e8aed6fcc1e981ca8305b4c30e274aa5cf51ef85371c8991`  
		Last Modified: Fri, 10 Apr 2020 01:26:13 GMT  
		Size: 192.0 MB (192002046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ad90426f5e94468e5350486b7b3f4ecc9b041db07bfbcd9efbe0223322949e`  
		Last Modified: Fri, 10 Apr 2020 01:25:56 GMT  
		Size: 3.5 MB (3460302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7accbc76eae8e3ea306c54cb637d966c68781418ad6cc2743a724927482278`  
		Last Modified: Fri, 10 Apr 2020 01:25:55 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
