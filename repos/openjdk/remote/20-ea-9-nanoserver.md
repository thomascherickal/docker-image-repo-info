## `openjdk:20-ea-9-nanoserver`

```console
$ docker pull openjdk@sha256:f19aba69e399848ed81ab0351d4b65e0796850f561010edf45ac940435e3ae27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:20-ea-9-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:f4127bbdf834cb220f16b29f411836b560627bf452feb17fefab7345a2b6cce5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.3 MB (299290617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d9d35eff7ec6c73d7498b475cc0e85d32f9cb58f288a41111732016916ec7ad`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 15:52:36 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 13 Jul 2022 15:52:37 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 15:52:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 15:52:50 GMT
USER ContainerUser
# Mon, 08 Aug 2022 22:18:32 GMT
ENV JAVA_VERSION=20-ea+9
# Mon, 08 Aug 2022 22:18:47 GMT
COPY dir:9fae0ad30370f51fbd8bd197d75531e4251998576cf345dfc35198b407c9d8a5 in C:\openjdk-20 
# Mon, 08 Aug 2022 22:19:11 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 08 Aug 2022 22:19:12 GMT
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
	-	`sha256:a3c94d05d6baacbfa68cfb2958f0965811612f86860a0e4f86c3742cdbfbc022`  
		Last Modified: Mon, 18 Jul 2022 21:22:32 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae155d737666fa6fb6c74f820b3e7f2470d72055ea13febb624515fcec6e1f`  
		Last Modified: Mon, 18 Jul 2022 21:22:32 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf301cbd6754860321dd411bf1baa15e0ba0f68154452e0ffb84915c2340f3f`  
		Last Modified: Mon, 18 Jul 2022 21:22:32 GMT  
		Size: 73.1 KB (73119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb02d029b4db33c144b7edd2594c5c7df303b1ea68bf6135d5133634b910d307`  
		Last Modified: Mon, 18 Jul 2022 21:22:30 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec62112de8286f25075b497f782e14ba624b9e4592984e05fb482b6e9438cb81`  
		Last Modified: Mon, 08 Aug 2022 22:28:53 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2873dc06d81c8c55df72478baa5a77b5912426c99ce68705e9e6f4cca6efd474`  
		Last Modified: Mon, 08 Aug 2022 22:29:15 GMT  
		Size: 192.3 MB (192346568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92473675e8e9d2a57536139a9a6118ad4e5be493e3e9bad96abadbabece146d2`  
		Last Modified: Mon, 08 Aug 2022 22:28:54 GMT  
		Size: 3.7 MB (3708955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fea086d1777fc8cef9c1c1dc7a5f57a3d63f74f824d0137450dc074e4ec73d0`  
		Last Modified: Mon, 08 Aug 2022 22:28:53 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
