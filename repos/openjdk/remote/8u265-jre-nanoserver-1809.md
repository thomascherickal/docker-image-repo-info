## `openjdk:8u265-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:e5ea4d80f8e5d09ef9a1c8e132ea118ded87a71054c5f4da6d64f4953d115303
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `openjdk:8u265-jre-nanoserver-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull openjdk@sha256:25c742fd22a226ace25d07540dcb90cb34e7dc4bf38ba326ba87905248035969
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138559827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d7873213ef35606085a9ff798e75ef4ebdc0ca2c9140485b260ac3f5abcc2db`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 06 Aug 2020 01:28:42 GMT
RUN Apply image 1809-amd64
# Wed, 12 Aug 2020 15:28:05 GMT
SHELL [cmd /s /c]
# Wed, 12 Aug 2020 16:01:37 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 12 Aug 2020 16:01:38 GMT
USER ContainerAdministrator
# Wed, 12 Aug 2020 16:01:48 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 12 Aug 2020 16:01:49 GMT
USER ContainerUser
# Wed, 12 Aug 2020 16:01:49 GMT
ENV JAVA_VERSION=8u265
# Wed, 12 Aug 2020 16:05:31 GMT
COPY dir:f9cdcac6b6965117d0bbadf86b5d0b55237954c067839a8e6ad0130705a48c8f in C:\openjdk-8 
# Wed, 12 Aug 2020 16:05:46 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:ce1c649a3e5b5b5449776d4afce631c673cade12336ccb5a38a0aac7c9d8b2bc`  
		Size: 101.0 MB (100984944 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1c7c341c7a3d0c7b6e849b6faec560815682d07ce87df2e4d1e83f928aab306b`  
		Last Modified: Wed, 12 Aug 2020 16:10:21 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4daf365d1451ee22d41b366a1ff5ae969d68435a4891cc5058e83d868b008eb`  
		Last Modified: Wed, 12 Aug 2020 16:23:30 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca485eb3d3fbc53b7bfe83c1550f9bec33fdc0153a7e297dbe84fc77f5c310a`  
		Last Modified: Wed, 12 Aug 2020 16:23:30 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a7252510ed8c3f762146994311ff0bed65ea719de5018c2f7c41e62543c26f`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 66.5 KB (66516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3df101f8092504a16a2b624e67e78b3fa8131c3908c1c309d5f6d70537afedd`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 935.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae04b3252587787aa96faab00ea2ab17d328bf541c96c8e11997c5095fd6aaa6`  
		Last Modified: Wed, 12 Aug 2020 16:23:28 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f5c3898163ce74833db803257620998b1d161cdd90021a4d778691a8ec8f08`  
		Last Modified: Wed, 12 Aug 2020 16:24:46 GMT  
		Size: 37.4 MB (37425880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda5ffbd4482bf0e67a392a4e0c9602dd9dc06b27cc6536b79711557bbd4261c`  
		Last Modified: Wed, 12 Aug 2020 16:24:40 GMT  
		Size: 78.0 KB (78044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
