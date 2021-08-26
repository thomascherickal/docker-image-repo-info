## `openjdk:nanoserver-1809`

```console
$ docker pull openjdk@sha256:c7b5d268111495f561c881d7c9d25ad16c02967ea443011a27e32b57c4958cfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:572fe098ab6f709302d01302f2c0f07c16730aa5d518f8ee6f4b77240d8d6a1c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.6 MB (286585919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7516aa0f41e3c8e7cb43ff2b1501dd9588dfb31f6f37bfe14834e319fcd91d2a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 17:18:00 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 25 Aug 2021 17:18:01 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 17:18:10 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 25 Aug 2021 17:18:10 GMT
USER ContainerUser
# Wed, 25 Aug 2021 17:18:11 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 25 Aug 2021 17:18:26 GMT
COPY dir:cb0fff7e1eb7273b9cd408e88cd60c60a3923c3595eb85b84f5ecaf2afd41761 in C:\openjdk-16 
# Wed, 25 Aug 2021 17:18:43 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 25 Aug 2021 17:18:43 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a975880c6d47e0333c4332c20ed02c496a0eb9a0b5542d91def6e578962fde5`  
		Last Modified: Thu, 26 Aug 2021 00:43:35 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facaf23bf7188445c948beb8083fafd70209da02e8e6f2cf9fb4d9e3b13dee00`  
		Last Modified: Thu, 26 Aug 2021 00:43:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefb0e311d4567d14f35f806c4fe3b643a3ba2b049ddf552022f562c561cc230`  
		Last Modified: Thu, 26 Aug 2021 00:43:35 GMT  
		Size: 68.4 KB (68385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdf691cc0bf8887e7d3e048517304972a26b2f486d8a8f597c8835457103f41`  
		Last Modified: Thu, 26 Aug 2021 00:43:33 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626ed8052e1ddd078ebcccf00463c851fdccdc6515701a8bcc39f44b421228b3`  
		Last Modified: Thu, 26 Aug 2021 00:43:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac05bb3123602f0b020378622848dc88788b4ebb862063ec4478c1068402b65e`  
		Last Modified: Thu, 26 Aug 2021 00:43:52 GMT  
		Size: 180.1 MB (180103167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ddcac6e4cec42f6fda5111e711abd4514ab18a07a1387416ef40193e0459f9`  
		Last Modified: Thu, 26 Aug 2021 00:43:34 GMT  
		Size: 3.7 MB (3666365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa82a64c3f5c8e2967cd25e59001b843551620ba3a95851ae8fae086e6041b5f`  
		Last Modified: Thu, 26 Aug 2021 00:43:33 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
