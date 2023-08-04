## `openjdk:22-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:42cd067a2c94ae7d26c195d6a3bf474ca9c49969efba60c63c20777e8ba614c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4645; amd64

### `openjdk:22-ea-nanoserver-1809` - windows version 10.0.17763.4645; amd64

```console
$ docker pull openjdk@sha256:ad8077c0dad430b67a94861cf451f8138999d0b7538a3bd937e6446be292d02c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.2 MB (307232545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea7d2bab2f311df17122d8d7ba2d3f58f5f7497542428f5d663694cd76de344`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Fri, 07 Jul 2023 07:42:59 GMT
RUN Apply image 10.0.17763.4645
# Thu, 13 Jul 2023 21:36:32 GMT
SHELL [cmd /s /c]
# Fri, 14 Jul 2023 00:14:58 GMT
ENV JAVA_HOME=C:\openjdk-22
# Fri, 14 Jul 2023 00:14:58 GMT
USER ContainerAdministrator
# Fri, 14 Jul 2023 00:15:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Fri, 14 Jul 2023 00:15:09 GMT
USER ContainerUser
# Fri, 04 Aug 2023 00:18:32 GMT
ENV JAVA_VERSION=22-ea+9
# Fri, 04 Aug 2023 00:18:51 GMT
COPY dir:6a23f2ebf681c4c32ab25d2a9e21b8cc95ce17229ce3a9322148fc1dab64b4fc in C:\openjdk-22 
# Fri, 04 Aug 2023 00:19:10 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 04 Aug 2023 00:19:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c5b06ba65934bcf850a1a54ecf4b3da34d3e6d6c8e90dbc897719c3ea377c8a`  
		Last Modified: Tue, 11 Jul 2023 17:31:37 GMT  
		Size: 104.4 MB (104408241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13c473988daf5951866dd9b290bd6417227c1d7df6e811cfe11438d033a1eba`  
		Last Modified: Thu, 13 Jul 2023 22:19:06 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544d6fd540738704e91e0cdf5ce429fe06193ca6f57b912ecd37720a5398c73e`  
		Last Modified: Fri, 14 Jul 2023 00:23:01 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184aebbaa7a5b561357f50ab1e278ddea12853b5513f6ccee076e8977ee17cb5`  
		Last Modified: Fri, 14 Jul 2023 00:23:00 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f517a720df0787d39ebc3c54f30149bad465e8af46947e6dd7c609c5c63d3ef3`  
		Last Modified: Fri, 14 Jul 2023 00:23:00 GMT  
		Size: 71.4 KB (71362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ee6f2b90fa1d7c818530d35c4808f44d5fa2414919c02d26f5b7db881751ed`  
		Last Modified: Fri, 14 Jul 2023 00:22:58 GMT  
		Size: 1.1 KB (1115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d941a7bc31a86edb0005e3f1174cfb65b0c0067eb063a86e580da7eb885f7d2`  
		Last Modified: Fri, 04 Aug 2023 00:25:39 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bc204b1917653c5923e226dd5df606298ec652586ce2c244ec99bc70c0589f`  
		Last Modified: Fri, 04 Aug 2023 00:26:00 GMT  
		Size: 198.9 MB (198902418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15a69ba21b69f08c6c14e5447ae014bc88928de9127a6aeef2eacbbd4b6a15`  
		Last Modified: Fri, 04 Aug 2023 00:25:40 GMT  
		Size: 3.8 MB (3843770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762f8dfe643da7c8893f4a28717e7f2c14ce36fc7e205c4e8d9a09df3d40d9e7`  
		Last Modified: Fri, 04 Aug 2023 00:25:41 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
