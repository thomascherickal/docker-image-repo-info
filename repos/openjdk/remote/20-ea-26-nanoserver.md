## `openjdk:20-ea-26-nanoserver`

```console
$ docker pull openjdk@sha256:68ddd0e746bc8da4008fc3a675d9cb46e8c2e7de1a2d3a35a0648486f5a2880b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `openjdk:20-ea-26-nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull openjdk@sha256:4c40256209c8d84cbb2e792d2aa5a29b697d78f07ff6d10b4645357e914e2ae3
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303499803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c105c7d651f86f2a350b8b3d21a933adce5fbe2e71241af5025d15794bdedd4d`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Tue, 08 Nov 2022 18:36:25 GMT
SHELL [cmd /s /c]
# Wed, 09 Nov 2022 17:26:48 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 09 Nov 2022 17:26:49 GMT
USER ContainerAdministrator
# Wed, 09 Nov 2022 17:27:06 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Nov 2022 17:27:07 GMT
USER ContainerUser
# Fri, 02 Dec 2022 00:19:11 GMT
ENV JAVA_VERSION=20-ea+26
# Fri, 02 Dec 2022 00:19:25 GMT
COPY dir:07fa926bbfd980a46e5c4dd43d42d0fc67057c4b39276db98dda93b2d7b4dc72 in C:\openjdk-20 
# Fri, 02 Dec 2022 00:19:57 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 02 Dec 2022 00:19:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e8f4bb4b79b67857c1e4ac5c66026fd5ff5badbde5a8b59b11251b02699586`  
		Last Modified: Tue, 08 Nov 2022 19:44:52 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5380ecadb3b5072bd5e7cf41fa446b5ae89ef7d71fde34772d7b32062aca954b`  
		Last Modified: Wed, 09 Nov 2022 17:37:09 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19002dcea365821038023716e28374a8210ac45b5a63b539639130ad9b6bd8`  
		Last Modified: Wed, 09 Nov 2022 17:37:08 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc05d65ddfbc35592002f4ae7726cad3fa9b8777ac1f0cbb66bad8963c18cc7`  
		Last Modified: Wed, 09 Nov 2022 17:37:08 GMT  
		Size: 74.7 KB (74716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0517802e30312d5724623bf6cc9fe338f7330d522b267fad48ae4f85da52072`  
		Last Modified: Wed, 09 Nov 2022 17:37:06 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a647b61761ba49ff959596279498f289b84838b62586dc76c0632a4af25f3a`  
		Last Modified: Fri, 02 Dec 2022 00:23:06 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffee173c7d38d77d3516a9ec17c41515adfad0ea25ae19d157703517452215a`  
		Last Modified: Fri, 02 Dec 2022 00:23:28 GMT  
		Size: 192.9 MB (192912383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e958c803aa47f6848a524507c8b2c82d159a06ac310e69751fc503a8dfc09a`  
		Last Modified: Fri, 02 Dec 2022 00:23:07 GMT  
		Size: 3.8 MB (3782617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f3dbc8c4cff2f63fe2a1da3fb5c89db8e71aeb901cc7c39371b193dd7dd6ac`  
		Last Modified: Fri, 02 Dec 2022 00:23:06 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
