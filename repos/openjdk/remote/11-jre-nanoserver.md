## `openjdk:11-jre-nanoserver`

```console
$ docker pull openjdk@sha256:db6b3ecbc73359c6b8018b76dfdfe62abc27d4eb446e54eb44f31071091d852e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `openjdk:11-jre-nanoserver` - windows version 10.0.17763.3165; amd64

```console
$ docker pull openjdk@sha256:dda28dc9087fdc1cdac7f00b5b678ca7eaaad26c3399d9116fa70fbedf71d2d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.0 MB (141995487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdbf7b07e2cb3b40e5bb1f746386a7cfa7a9bc85e556cca461a108bf0a77db36`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 14:50:41 GMT
SHELL [cmd /s /c]
# Wed, 13 Jul 2022 16:06:40 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Jul 2022 16:06:41 GMT
USER ContainerAdministrator
# Wed, 13 Jul 2022 16:06:49 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Jul 2022 16:06:49 GMT
USER ContainerUser
# Mon, 25 Jul 2022 20:20:20 GMT
ENV JAVA_VERSION=11.0.16
# Mon, 25 Jul 2022 20:23:25 GMT
COPY dir:d6bf51b9863c520625211f12dc2b206c3a8752f0afd5533cf5bbbdf42ae36957 in C:\openjdk-11 
# Mon, 25 Jul 2022 20:23:37 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3b09c07c6aeead64423fdefc240fe2e1b6330c96732fd2705113030da84416be`  
		Last Modified: Mon, 18 Jul 2022 21:22:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1234d8139b62fe1cc2af73e6f7e19087c38bbf27b1301126e4825445a53129ba`  
		Last Modified: Mon, 18 Jul 2022 21:29:22 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fb8775c7c189c574b2c2e9559d8e0069174344caf6a8e82a8a8311e9b46649`  
		Last Modified: Mon, 18 Jul 2022 21:29:22 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e18300deee27181a3e362a7857b5e4f7d95ad751f96a0b3fff63f97d8ba0f`  
		Last Modified: Mon, 18 Jul 2022 21:29:22 GMT  
		Size: 69.0 KB (68975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31f1cf222f09294611ee30eb57920d0e6ee6e7aecd5a3d0d0ce758b70f63b33`  
		Last Modified: Mon, 18 Jul 2022 21:29:20 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944b48a8d4fa16e483c85b0f55f7c05cc752e4d2dba358860ad25a82e47bb8b3`  
		Last Modified: Mon, 25 Jul 2022 20:34:42 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d7f174d10dd2431823aeec70575682507f3f06ef68ce58910c00748225d741`  
		Last Modified: Mon, 25 Jul 2022 20:36:10 GMT  
		Size: 38.7 MB (38679651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3951e2d67d258818975209035a9d6b7dee09119dfa0b3327a32664649680e4c1`  
		Last Modified: Mon, 25 Jul 2022 20:36:03 GMT  
		Size: 86.2 KB (86194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
