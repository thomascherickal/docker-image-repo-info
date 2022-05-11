## `openjdk:11-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c03992a778d5adff8dfdb768acccd484b1f9bf2169129b95dc6e2a6231e961dd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:11-jre-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:ab0365640f7371f6fb775f77508c7975c7962f270b4b0b56f44e0bf9b0653309
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.8 MB (142754462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537de492fd80e538edcb14da10daa5941ecd5474d390c51a5402b73cac3f9551`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:42:59 GMT
ENV JAVA_HOME=C:\openjdk-11
# Wed, 11 May 2022 15:43:00 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:43:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:43:09 GMT
USER ContainerUser
# Wed, 11 May 2022 15:43:09 GMT
ENV JAVA_VERSION=11.0.15
# Wed, 11 May 2022 15:46:09 GMT
COPY dir:b19a7bc4e0a7772217140b5b5a40fc0497b9874821c6267cef822ccc10258697 in C:\openjdk-11 
# Wed, 11 May 2022 15:46:39 GMT
RUN echo Verifying install ... 	&& echo   java --version && java --version 	&& echo Complete.
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6def212f703808f6360427fa8ccb305eecb76f9f05c0e56297cf3089475ff71`  
		Last Modified: Wed, 11 May 2022 16:20:01 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff467abade7a5781679aa340b9381730fbd361c2e8b612b46f4b901659e0eeea`  
		Last Modified: Wed, 11 May 2022 16:20:01 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39110621289c17286b4f7fe1588a33f74aae12b4fd06ac77ec209ac6310bff3e`  
		Last Modified: Wed, 11 May 2022 16:20:01 GMT  
		Size: 75.9 KB (75907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee1ec743653236f008be7e72e243218dcdc2da5da92a01414a173050a36c49`  
		Last Modified: Wed, 11 May 2022 16:19:59 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8efe86a72b28d1026389dd24c48f45d0b041cfffa893a669d40fb9764418b9d2`  
		Last Modified: Wed, 11 May 2022 16:19:59 GMT  
		Size: 1.0 KB (1032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301e16c2baec00b3665ef89e1929492b8fd49d729ae8ce932790fb41106944ba`  
		Last Modified: Wed, 11 May 2022 16:23:16 GMT  
		Size: 39.5 MB (39490409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb9da5fc98679f230d4f93df244508e2768c8aaac6f0b3d8a38741d7cc59da2`  
		Last Modified: Wed, 11 May 2022 16:22:32 GMT  
		Size: 49.0 KB (49035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
