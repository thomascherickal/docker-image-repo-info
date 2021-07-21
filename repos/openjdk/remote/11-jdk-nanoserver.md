## `openjdk:11-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:e738697e593c93826c762ef21efa9ae4488f991ab58f779bbd341b266782b5db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `openjdk:11-jdk-nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull openjdk@sha256:77022211b2e3d0211752aeb6d87bb4b1f186a044299bea09eb90b4a472047690
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.0 MB (293991466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ccec9af44c4a8d10423418b2cb6431b35f85f4d599464d18ba159a0a6ee63d8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:53:30 GMT
SHELL [cmd /s /c]
# Wed, 14 Jul 2021 03:18:47 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 14 Jul 2021 03:18:49 GMT
USER ContainerAdministrator
# Wed, 14 Jul 2021 03:19:04 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Jul 2021 03:19:06 GMT
USER ContainerUser
# Wed, 21 Jul 2021 18:20:23 GMT
ENV JAVA_VERSION=11.0.12
# Wed, 21 Jul 2021 18:20:42 GMT
COPY dir:8d687b3cc71690b95b3812413f66d278c1566215f055e8d2ed9ac022b638e9a3 in C:\openjdk-11 
# Wed, 21 Jul 2021 18:21:27 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 21 Jul 2021 18:21:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:78d8754fb12dd351c91bed29d92c703cddb135a78d8f056b6a3bf13a251c1d2d`  
		Last Modified: Wed, 14 Jul 2021 03:42:27 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe8e02e3faa5ffe937981f50a3277b0002846576df467ba8249d6f2b31304d8`  
		Last Modified: Wed, 14 Jul 2021 03:55:22 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee577adaec81f9c2fc86655503a1a6c8f61898b66788f16a75115f54b86a70`  
		Last Modified: Wed, 14 Jul 2021 03:55:22 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1095968790bd405f2a988693d7983d88c75c1c828991e0bef3dc30db4960240`  
		Last Modified: Wed, 14 Jul 2021 03:55:22 GMT  
		Size: 65.2 KB (65235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0600a4c7c20741a18bd07b8b940ddd0dbe295deae0754a43febd281fc6b81e`  
		Last Modified: Wed, 14 Jul 2021 03:55:19 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e244da682e9c17e9e764a7e690aca2b9871c8dbbbcb6e1768aa04a81da69015b`  
		Last Modified: Wed, 21 Jul 2021 18:39:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c67a418e4298291850e6ef70a236b5b24be6a335d1e869225bf102967366a8d`  
		Last Modified: Wed, 21 Jul 2021 18:39:31 GMT  
		Size: 191.1 MB (191115635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64acbdc1c6f6440646de1442a77fb00c3c5693d8139815179a6c4d12748154ee`  
		Last Modified: Wed, 21 Jul 2021 18:39:08 GMT  
		Size: 78.0 KB (77978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5d216fe63d10d56cf53bafdc4222c97fe104df68e5c1969c2906a0929ea9b3`  
		Last Modified: Wed, 21 Jul 2021 18:39:09 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
