## `openjdk:20-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:17e8ca91d8bb0e0c8c3f77d427e73cf9a610f936890b9acecc5f0a9dee3de9c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:20-ea-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:257b3ca2961474116426d2dbbb16cf635d3e155183bf861b5ba566f5b21920df
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.3 MB (299327925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ecb78d8266450503eaf3b6d389118370393eb8628168f039541a185bac8458f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:00:08 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 10 Aug 2022 17:00:09 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:00:18 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:00:18 GMT
USER ContainerUser
# Wed, 10 Aug 2022 17:00:19 GMT
ENV JAVA_VERSION=20-ea+9
# Wed, 10 Aug 2022 17:00:34 GMT
COPY dir:9fae0ad30370f51fbd8bd197d75531e4251998576cf345dfc35198b407c9d8a5 in C:\openjdk-20 
# Wed, 10 Aug 2022 17:00:47 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 10 Aug 2022 17:00:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0f4438539876006761cb687527bd8cb94cc7a273cf8bb47563981044f2e1771e`  
		Last Modified: Wed, 10 Aug 2022 16:38:40 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151c855f0d179e8547473b92e962fb22b468853448fe0849dadde3526c52aceb`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3386f9f9687d0a909a16379459e37c52a2de2070297d81d4167037a0602e3e86`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28092505f98fc516238306cba539a3a8a6d7f48ca19dc6e6c3cca668dc6f466c`  
		Last Modified: Wed, 10 Aug 2022 17:28:35 GMT  
		Size: 75.6 KB (75615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dfea14a612ecceac1dd16eaa1da4863923aa41d796fd4f9c1fae46d918d4299`  
		Last Modified: Wed, 10 Aug 2022 17:28:33 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fca8e12bd43676000ee6ec7661729ee5fa64d581e76605146e84b1833be3bf4`  
		Last Modified: Wed, 10 Aug 2022 17:28:32 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1477f44e332abd34331b00c6efa5f491133920e955f6a7ad2d189c80b9f4efeb`  
		Last Modified: Wed, 10 Aug 2022 17:28:55 GMT  
		Size: 192.3 MB (192334740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cab4e6241ce706ed9237743807979b3179b2aa396e2411416f4b043c20fd4b`  
		Last Modified: Wed, 10 Aug 2022 17:28:34 GMT  
		Size: 3.7 MB (3706446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf40917da92f52c73782af053eb153506ed7346d58ad2404a7cce82e5342ad01`  
		Last Modified: Wed, 10 Aug 2022 17:28:32 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
