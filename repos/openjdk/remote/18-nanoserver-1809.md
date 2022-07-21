## `openjdk:18-nanoserver-1809`

```console
$ docker pull openjdk@sha256:d55a0138503f0c76c477bd8a5ed1e8bae36edd29fa568479bcfa3f769c008e4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:18-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:4544df86f1f4ba3e846ec5cdcd823be86d2a78d2e96324a2b4f523c0d9dcc89f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (290992078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4a44b98dd479f0db6a8f200f4e7a7e234715dfc43c711ca69a9f4c9e192111e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 16:02:00 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 13 Jul 2022 16:02:01 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 16:02:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 16:02:09 GMT
USER ContainerUser
# Thu, 21 Jul 2022 00:20:00 GMT
ENV JAVA_VERSION=18.0.2
# Thu, 21 Jul 2022 00:20:15 GMT
COPY dir:1a22cafd1c3a73c07e75460ef8cc20669902f9a162797035a29e2b4c98b82396 in C:\openjdk-18 
# Thu, 21 Jul 2022 00:20:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 21 Jul 2022 00:20:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90d0b31a46eadf635992b6a5525391cd83217e1f005db119212fe5e339d7e8c6`  
		Last Modified: Mon, 18 Jul 2022 21:27:11 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c78cfac735d9ca0503eacb60a31c17de68b5f2aa1e5880b055a8a4ed2139a6f`  
		Last Modified: Mon, 18 Jul 2022 21:27:11 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e679483c6d631da7bd390ecec3dcf2a5f80ebd13b368fe3047235ffd417546`  
		Last Modified: Mon, 18 Jul 2022 21:27:11 GMT  
		Size: 67.0 KB (67046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440b0951fe6ccabbd13a8594ec03367bcc9b274b48a7992722931b6601f96d81`  
		Last Modified: Mon, 18 Jul 2022 21:27:09 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe8a29144fd6cffe2c0bda4cccb429df2903d6df6e2458ed719fd2571aad9f9`  
		Last Modified: Thu, 21 Jul 2022 01:25:47 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ab337e0e7784d6b3995bee69873d7cb51a1c2e6730b4b37cf378918fe59f8a`  
		Last Modified: Thu, 21 Jul 2022 01:26:10 GMT  
		Size: 184.2 MB (184214398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06382f24cb7099eea98f550aa458e7ca9e39d02ac21a4ff00c9a91a31aed365`  
		Last Modified: Thu, 21 Jul 2022 01:25:48 GMT  
		Size: 3.5 MB (3548685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1999bed8d1ebe8c1db811b712ebbe3167defda83a29602a5ce9030262a79a6e4`  
		Last Modified: Thu, 21 Jul 2022 01:25:47 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
