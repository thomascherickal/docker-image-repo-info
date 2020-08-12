## `openjdk:15-nanoserver-1809`

```console
$ docker pull openjdk@sha256:085eb03a9d4da35021c10573def77368e007b3a751a00f213e7dbea5f185f5f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:15-nanoserver-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:89ef1517fb63d5b5dc16825eacf5a0ea65675ce34331a49c0fcb17abe0605c0c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295899107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4867db0e5154eebe54ef32ab8786649d6c3a6bd6d6b80b7bc486a7a9c4e38d79`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:28:05 GMT
SHELL [cmd /s /c]
# Wed, 12 Aug 2020 15:35:41 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 12 Aug 2020 15:35:42 GMT
USER ContainerAdministrator
# Wed, 12 Aug 2020 15:35:52 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 12 Aug 2020 15:35:53 GMT
USER ContainerUser
# Wed, 12 Aug 2020 15:35:53 GMT
ENV JAVA_VERSION=15
# Wed, 12 Aug 2020 15:36:33 GMT
COPY dir:4c7563c7b2e040444227132d1a1c3dae3372f0cf26f8929954f8261ead9f7656 in C:\openjdk-15 
# Wed, 12 Aug 2020 15:36:53 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 12 Aug 2020 15:36:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1c7c341c7a3d0c7b6e849b6faec560815682d07ce87df2e4d1e83f928aab306b`  
		Last Modified: Wed, 12 Aug 2020 16:10:21 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908c3f69eea8e2eeda13b3a2bc36cb5bddc8f02e4add43f8074ea08d0254ab6b`  
		Last Modified: Wed, 12 Aug 2020 16:12:20 GMT  
		Size: 831.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfa99a5cb7aa58c10707652cd6441f23958888cdb3de7292e9f805230737eb0`  
		Last Modified: Wed, 12 Aug 2020 16:12:20 GMT  
		Size: 827.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21f16c0f1eef9755ced9deac574ce43f9d82e3b5d8f235ff69a39d2d3ada378`  
		Last Modified: Wed, 12 Aug 2020 16:12:20 GMT  
		Size: 67.3 KB (67309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4d1d1646f8cee0a046ee309f0100de2962628c9942413c59f33e2eff3374ab`  
		Last Modified: Wed, 12 Aug 2020 16:12:17 GMT  
		Size: 842.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcb5d3af38d42a971343edc08139ef1411452f01359595908be6153bfb1b1b9`  
		Last Modified: Wed, 12 Aug 2020 16:12:17 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b1afd7e76844b27ba1fc05c72f7bd3c1a73d148da8a0bff98bcb2cf48ef6aa`  
		Last Modified: Wed, 12 Aug 2020 16:12:40 GMT  
		Size: 191.4 MB (191357188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e8fe53ebc7a678548b2d018f2eb90f218c0d01a8208fc0164136eb448662c`  
		Last Modified: Wed, 12 Aug 2020 16:12:18 GMT  
		Size: 3.5 MB (3484597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9e8c98f5bea818d87cfdf458f4025ceaa437ddc2b34f9965ce3b6619253f10`  
		Last Modified: Wed, 12 Aug 2020 16:12:17 GMT  
		Size: 862.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
