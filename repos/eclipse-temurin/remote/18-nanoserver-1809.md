## `eclipse-temurin:18-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:037afe1e4fe3d4c241445fa5991c46f81194221aaa0d8b75e1348db90965d6c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `eclipse-temurin:18-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull eclipse-temurin@sha256:95f401f231f06f2a083643f3839c1104ebe9bccf6970c70a1af90cdf20db2396
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.1 MB (293145518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b45be1f88912568502582098d17a2d876e2bca41575dfa590083db59ce198b5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 04 May 2022 18:23:03 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 04 May 2022 18:23:04 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 04 May 2022 18:23:05 GMT
USER ContainerAdministrator
# Wed, 04 May 2022 18:23:11 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 04 May 2022 18:23:12 GMT
USER ContainerUser
# Wed, 04 May 2022 18:23:27 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 04 May 2022 18:23:41 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 04 May 2022 18:23:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1818cdab77f23e78fedaca52a20efe1c4ba35571fb089c70e1485124b9c6145`  
		Last Modified: Wed, 04 May 2022 18:33:30 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77646ae8dc09eb94667a43ea3487777f6cc340f4aaf6c909df70299066d9d371`  
		Last Modified: Wed, 04 May 2022 18:33:29 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7102f2da8b5b2796607c79458ec46fa80513872248c745ca845aca54bd2163`  
		Last Modified: Wed, 04 May 2022 18:33:30 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd66b464e0ea5b83f563c471243fc90144f3895080f5cdb204456348cdc10af`  
		Last Modified: Wed, 04 May 2022 18:33:27 GMT  
		Size: 72.4 KB (72386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362058c540505251e6ea236372b1a3e9b786fe60acaa0b59a4079cb357fb05bb`  
		Last Modified: Wed, 04 May 2022 18:33:27 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1041313182faac2a7422b91948474a3175f62a5b197873db75c1cd7881dd11`  
		Last Modified: Wed, 04 May 2022 18:33:47 GMT  
		Size: 186.4 MB (186415988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deea4a1f3cccecf59de35ec1c9f90d73a8b8005d94a56552c080988bffdac108`  
		Last Modified: Wed, 04 May 2022 18:33:31 GMT  
		Size: 3.6 MB (3554149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d263304a33e784a8851bf7d9dd3fedfca951342be053b90405c60d822869139`  
		Last Modified: Wed, 04 May 2022 18:33:27 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
