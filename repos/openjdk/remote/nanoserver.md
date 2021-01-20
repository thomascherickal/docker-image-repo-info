## `openjdk:nanoserver`

```console
$ docker pull openjdk@sha256:cb0173567506c625519a3534214626f79488776a4bb387c297e3d10781e7a300
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1697; amd64

### `openjdk:nanoserver` - windows version 10.0.17763.1697; amd64

```console
$ docker pull openjdk@sha256:82ca3717d64ca4ba3e2f56633fef21ccd91d9eed73281bc50a695601a57dc5a9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.3 MB (296339415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8137937de0356c1a708f8df73f94aeb298f13685b273d613b4b7f1583978cef`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Jan 2021 16:14:35 GMT
RUN Apply image 1809-amd64
# Wed, 13 Jan 2021 19:56:48 GMT
SHELL [cmd /s /c]
# Wed, 13 Jan 2021 20:42:55 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 13 Jan 2021 20:42:56 GMT
USER ContainerAdministrator
# Wed, 13 Jan 2021 20:43:07 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 13 Jan 2021 20:43:07 GMT
USER ContainerUser
# Wed, 20 Jan 2021 02:41:49 GMT
ENV JAVA_VERSION=15.0.2
# Wed, 20 Jan 2021 02:42:24 GMT
COPY dir:faf6f6b60355f43c9d304f91959c61fcd201df906c7d5f09f1cd84c7986207a8 in C:\openjdk-15 
# Wed, 20 Jan 2021 02:42:45 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 20 Jan 2021 02:42:46 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:62239e9aa1a352a20b0d4969c2b508b8a18d10e799d4db72e6f24ccbb2c724d9`  
		Size: 101.3 MB (101340070 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c2b6c001c337f812bceb3b03d15a70d1d9905540658e751e42f20f7cc0ddc819`  
		Last Modified: Wed, 13 Jan 2021 21:16:47 GMT  
		Size: 908.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b06e2760220b592d7223a535812762ce910e4e06c4b5c9d7a063dd227e80c4`  
		Last Modified: Wed, 13 Jan 2021 21:25:46 GMT  
		Size: 859.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05331d9e36f3b34b20230294798b851d181ef624007e98b2de364f49d828b12`  
		Last Modified: Wed, 13 Jan 2021 21:25:45 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2217464be837992891e2442451031cb999e6c2acee7eddc7bf59195c91acfd67`  
		Last Modified: Wed, 13 Jan 2021 21:25:44 GMT  
		Size: 66.5 KB (66517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec13ba6c204194c9ae26b5c4a1261c1de60235cb039258267fa4cc80c8ee84a`  
		Last Modified: Wed, 13 Jan 2021 21:25:41 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f509bf29c46010ac55ac2ccda86198e364fe00b1789c1a2eefa8ad9501efe6`  
		Last Modified: Wed, 20 Jan 2021 02:54:14 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c59701500efb90ac041d9ceab36de4351c1135ba58cc4c7ad2beecdfc851ad`  
		Last Modified: Wed, 20 Jan 2021 02:54:33 GMT  
		Size: 191.4 MB (191390044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e2730d6fa047056274c8a5fdf8f4e0e1e651b6247ea2199a2c23ff008cb5ac`  
		Last Modified: Wed, 20 Jan 2021 02:54:15 GMT  
		Size: 3.5 MB (3536999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d1f6e63e64b05214c0e64f0897c91b4535aa1843fcc3616c6746db759370a1`  
		Last Modified: Wed, 20 Jan 2021 02:54:14 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
