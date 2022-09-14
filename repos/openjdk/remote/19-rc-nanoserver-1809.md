## `openjdk:19-rc-nanoserver-1809`

```console
$ docker pull openjdk@sha256:70fb5cf8b879560e45b70e327a6950d6fc175fe26aef78103fe5ff2ea52641e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `openjdk:19-rc-nanoserver-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull openjdk@sha256:fe046aca2692d4c5f0db2a3c58a670500ff0991d6e90967c626752ab03bfd616
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.3 MB (298336689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c2aa5abd0d15d23f74c95ca967fdf6039a514c60ca00e4e330143e2ba9c64a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 09 Sep 2022 22:22:51 GMT
RUN Apply image 10.0.17763.3406
# Wed, 14 Sep 2022 16:03:00 GMT
SHELL [cmd /s /c]
# Wed, 14 Sep 2022 17:14:05 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 14 Sep 2022 17:14:05 GMT
USER ContainerAdministrator
# Wed, 14 Sep 2022 17:14:14 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Sep 2022 17:14:14 GMT
USER ContainerUser
# Wed, 14 Sep 2022 17:14:15 GMT
ENV JAVA_VERSION=19
# Wed, 14 Sep 2022 17:14:31 GMT
COPY dir:ad572564354aac78397e790af4fedd1886f683bcb0c086fecfa550483cfa75ad in C:\openjdk-19 
# Wed, 14 Sep 2022 17:14:48 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 14 Sep 2022 17:14:49 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bcd4ab6c304faa0a7f4e183705a7f6e4545b728788221d17886d2a507ea0a06d`  
		Size: 103.3 MB (103334221 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:233f09b2a52487084f2cfb5e06dac2815651432c9d37c729582f59cfcf66b243`  
		Last Modified: Wed, 14 Sep 2022 16:47:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8637b2712d96544e3c85916b38472d0a6a0a449e64420c4270602a23ab7d0c`  
		Last Modified: Wed, 14 Sep 2022 17:24:51 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb022cac421e4aa292167c8b43d05672a24561ede79864dd52e2a0ee87edbe0`  
		Last Modified: Wed, 14 Sep 2022 17:24:51 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebc9b5f0052e4c6b3e6698c6a3130561419f9adb2aec48b7f1da8978c865c02`  
		Last Modified: Wed, 14 Sep 2022 17:24:51 GMT  
		Size: 70.0 KB (70006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2872b9a8015a870253aebbb1b7749c0b5fd1984014814dc0f851f73e755fa08`  
		Last Modified: Wed, 14 Sep 2022 17:24:48 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00878cb840d2d99228abb9995cb142d20bb4d8fffbc47059dbe9345e4ebbd96d`  
		Last Modified: Wed, 14 Sep 2022 17:24:49 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6cb58d9ec037e61294092c9ebd36ddabb9901e00c343c20789d20397ecf93c`  
		Last Modified: Wed, 14 Sep 2022 17:25:08 GMT  
		Size: 191.2 MB (191206716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da65fa5989247ff806ad1ac9f4443367b76b63a88b79248cffa7c4f2fde780e3`  
		Last Modified: Wed, 14 Sep 2022 17:24:49 GMT  
		Size: 3.7 MB (3718868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15032e9ddda1a3e1610593e585a5f66acdf479b4e8fc55787edc587b7db7634c`  
		Last Modified: Wed, 14 Sep 2022 17:24:48 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
