## `openjdk:20-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:894cc6bb5e835765c3f270a64ba35db2448773b1125d8a16a522fc6782046111
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:20-ea-nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:2e7f91947b09e64bde4a1f29fbc0cb99a4752a50b4d2fed139b88cbe2874b160
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299178110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9afa7f086e42b045842c41be38a438c38e17256832fd87e76c789f0778f6d773`
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
# Fri, 29 Jul 2022 01:18:59 GMT
ENV JAVA_VERSION=20-ea+8
# Fri, 29 Jul 2022 01:19:15 GMT
COPY dir:b6bd0eeda56d9ccb0c6d383e67745e794067ea3d98b1964182063684e39c2e24 in C:\openjdk-20 
# Fri, 29 Jul 2022 01:19:39 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 29 Jul 2022 01:19:39 GMT
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
	-	`sha256:5cb3fa9983ed546016876d7981c8ecccd954b5c6993524b1cbbb6089e36d6baa`  
		Last Modified: Fri, 29 Jul 2022 03:21:18 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e02c95f80e023b779a9f0bd68af506feb047fb2ecc3ff754d2de1362f642324`  
		Last Modified: Fri, 29 Jul 2022 03:21:37 GMT  
		Size: 192.2 MB (192234054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72043e9f28b731f24717e072a2c6f9c163c74d3261c3ebf66e3bf2ecbfcfe2c0`  
		Last Modified: Fri, 29 Jul 2022 03:21:18 GMT  
		Size: 3.7 MB (3709219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd5d2ecbc7a205d079febe7475f3758b443d6ccd01777fc79d83b335249adb9`  
		Last Modified: Fri, 29 Jul 2022 03:21:18 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
