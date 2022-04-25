## `openjdk:11-jre-nanoserver`

```console
$ docker pull openjdk@sha256:3d5335f1039dbd30888eab2d9327ee34a994da232cb3f46b826fb59b7c8dce0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:11-jre-nanoserver` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:829fa9d6f687931cc75fc3bf17227881f5cd628fa793b1c8708c5971180b5f79
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142742856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943d09c7b9274ce399e016db670306210bf6711594a7e7f1f265bf072f111783`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:14:56 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 13 Apr 2022 17:14:57 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:15:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:15:03 GMT
USER ContainerUser
# Mon, 25 Apr 2022 18:30:27 GMT
ENV JAVA_VERSION=11.0.15
# Mon, 25 Apr 2022 18:33:46 GMT
COPY dir:b19a7bc4e0a7772217140b5b5a40fc0497b9874821c6267cef822ccc10258697 in C:\openjdk-11 
# Mon, 25 Apr 2022 18:33:56 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6fc97003d8b7f593fe071cf3ea64f3ce760cc060f3402bb6b1b849c040e222d5`  
		Size: 103.1 MB (103096169 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ea4009814dceb50337c66614a6008cfc2fb73ce53e62162bce071ef6ea1adf2d`  
		Last Modified: Wed, 13 Apr 2022 15:58:06 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849f82959ffa51b7fc97fc8d879a85b8b443d32aa27a8507f2200e370c4022f6`  
		Last Modified: Tue, 19 Apr 2022 01:11:33 GMT  
		Size: 1.1 KB (1052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302ab25e933bb29e0963abb16a53cff6a3f17aaa4d0de148077b06ab85fbb123`  
		Last Modified: Tue, 19 Apr 2022 01:11:33 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5f0ad271138cceb8261825016c3345ae53a44e0d7eb7df18a792fa61d5e5b6`  
		Last Modified: Tue, 19 Apr 2022 01:11:33 GMT  
		Size: 69.7 KB (69695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e23c499a1f064ee45af7c5b2696ec11f98304ec5ae5b878e24508df3ff0551c`  
		Last Modified: Tue, 19 Apr 2022 01:11:31 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37b751eb3aa1d74a85ae8b76e36a8d55bf328ebbdedde3f8b0a34061c805ac6`  
		Last Modified: Mon, 25 Apr 2022 20:31:09 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e759b1268d0a0b0b0f46483827cc018e3a56e2ab31d6059bae3732ee1ca747`  
		Last Modified: Mon, 25 Apr 2022 20:36:25 GMT  
		Size: 39.5 MB (39489343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d865e6b226182ba42167d0246618ab13697dbd7682fc636233382604cc165af2`  
		Last Modified: Mon, 25 Apr 2022 20:36:17 GMT  
		Size: 82.4 KB (82366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
