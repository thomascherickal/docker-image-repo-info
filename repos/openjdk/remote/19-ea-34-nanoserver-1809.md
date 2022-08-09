## `openjdk:19-ea-34-nanoserver-1809`

```console
$ docker pull openjdk@sha256:33e9e067f2944b156092f26df30bfe8851b773cc0054ed055822ec95640b8d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:19-ea-34-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:575bbccea0d5b2a17340c4ed894771de2404e0543ce71223c0de08d0fd7b917f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298166664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b10d100a91fb2532b02ebc4f105b445013766b4a7b451b9d03dc70f74af2e5ef`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:57:38 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Jul 2022 15:57:39 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:57:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 15:57:47 GMT
USER ContainerUser
# Mon, 08 Aug 2022 22:22:10 GMT
ENV JAVA_VERSION=19-ea+34
# Mon, 08 Aug 2022 22:22:25 GMT
COPY dir:a915abe9a325cfc0cb6f8cb6819a212af006cc12f498bc43c7ec9f4f4c627c43 in C:\openjdk-19 
# Mon, 08 Aug 2022 22:22:43 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 08 Aug 2022 22:22:44 GMT
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
	-	`sha256:a24a8dc780930fe59a9967fb76b10b2fb2ac36ff76c3697586a3df823f25ab8d`  
		Last Modified: Mon, 18 Jul 2022 21:24:44 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1582b9bf63a2d6ede0a45ecb506c093cf9a09b81e8de25dd46c5bffa9c7d94`  
		Last Modified: Mon, 18 Jul 2022 21:24:43 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4239363179c317c462b5006da97ce6faa8c7e4256719a99f4c3dd0cb7a4b524f`  
		Last Modified: Mon, 18 Jul 2022 21:24:43 GMT  
		Size: 69.0 KB (69030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dd52e79d9b5ebce7877fd3f3e42eb3c3cfae509d375aa166c3a01cb8e29a9`  
		Last Modified: Mon, 18 Jul 2022 21:24:41 GMT  
		Size: 1.1 KB (1065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db90ffb0a1e7630857c5246ddc3ad6593e745fdd79330929d76c6db74431f70b`  
		Last Modified: Mon, 08 Aug 2022 22:30:59 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa29b4635aba10faf6c406caec68b24ba73155c9ebed8d8dcfcc915af3343e33`  
		Last Modified: Mon, 08 Aug 2022 22:31:19 GMT  
		Size: 191.2 MB (191212671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524948f0cccc9a388d8a43732bdd74e8f2368ec393b2c1ca8ba8898ad0f4d8aa`  
		Last Modified: Mon, 08 Aug 2022 22:31:00 GMT  
		Size: 3.7 MB (3723372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8977245cdffc0b38caea2db3df7dd73d2ea8d1aca3fd471285c0c14c7073c0`  
		Last Modified: Mon, 08 Aug 2022 22:30:59 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
