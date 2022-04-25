## `openjdk:19-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:096d6fb143329dce7f71aed8be91a594e2cd3cda8d60e144db0959621574cae5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `openjdk:19-ea-jdk-nanoserver-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull openjdk@sha256:bb5ddb012da3593ea6431ede5986cd3520a31229b95b5d931d732856dccb4276
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.5 MB (296464112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48dffabe2f41d0dc87050c252c765cbddf2546e71444ab6c3ad8d307664fa6f6`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Mon, 04 Apr 2022 10:52:49 GMT
RUN Apply image 1809-amd64
# Wed, 13 Apr 2022 15:16:11 GMT
SHELL [cmd /s /c]
# Wed, 13 Apr 2022 17:00:37 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 13 Apr 2022 17:00:38 GMT
USER ContainerAdministrator
# Wed, 13 Apr 2022 17:00:44 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 13 Apr 2022 17:00:44 GMT
USER ContainerUser
# Mon, 25 Apr 2022 18:26:13 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:26:28 GMT
COPY dir:1e969d9cdb5d7d57826d3098ae8f95959a0181a9dc44cda5d1bd3047ff24fdde in C:\openjdk-19 
# Mon, 25 Apr 2022 18:26:44 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Mon, 25 Apr 2022 18:26:44 GMT
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
	-	`sha256:be4644baf69a04abfb80da969c1fb009552c461553f3672bd4e787c0ac7c37ea`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61095df7d33e436b0d9cb0052f433e155a897f4278b9dc0a8d13582d6cad38ad`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2110ca10faf88314f61157ce6bfeb157b8b8eebd74be6f0a78f2f7b82c514a`  
		Last Modified: Tue, 19 Apr 2022 00:53:51 GMT  
		Size: 68.8 KB (68813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd03d4716f16fd9ebec77b5cf5099ed25d889884b5a06da589ce896a7db47a15`  
		Last Modified: Tue, 19 Apr 2022 00:53:49 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a7969b97cac36e74af7b1ec3c1e19f692e56df625846a96faf6afc28d04b6e`  
		Last Modified: Mon, 25 Apr 2022 20:25:47 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5808f1126b0ed62ba0a5eb96cfb0194b79c1ddc9099bea8e974013e1b6ebadbd`  
		Last Modified: Mon, 25 Apr 2022 20:29:14 GMT  
		Size: 189.7 MB (189710177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f7b62eba3d5c67b80065c05f6ce1eff9d60692fe59f799de00e926032508a`  
		Last Modified: Mon, 25 Apr 2022 20:25:48 GMT  
		Size: 3.6 MB (3582210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c466d31ab00f09b528848d76a32f51920665a6ecdb1f1579627f80d9c334488`  
		Last Modified: Mon, 25 Apr 2022 20:25:47 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
