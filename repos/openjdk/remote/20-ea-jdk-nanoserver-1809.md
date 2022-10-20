## `openjdk:20-ea-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f899d7ad84f1c17a645eb8ca9508d8d0832ca41fdda9f96691c98ba5beae8277
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `openjdk:20-ea-jdk-nanoserver-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull openjdk@sha256:91cb24e9a7f51f4a18f00203046384a0269f6ed19cd3bd16dcb742e69ef65e2f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.3 MB (299287920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2a7ee8657cf613c59cb468fe29f865872d669f6994ad36d5cbfcb95baddf2a`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 08 Oct 2022 01:37:47 GMT
RUN Apply image 10.0.17763.3532
# Wed, 12 Oct 2022 15:20:49 GMT
SHELL [cmd /s /c]
# Wed, 12 Oct 2022 16:43:51 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 12 Oct 2022 16:43:51 GMT
USER ContainerAdministrator
# Wed, 12 Oct 2022 16:44:02 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 12 Oct 2022 16:44:03 GMT
USER ContainerUser
# Thu, 20 Oct 2022 20:20:41 GMT
ENV JAVA_VERSION=20-ea+20
# Thu, 20 Oct 2022 20:20:56 GMT
COPY dir:ba03fe7c24763c5fe51458d34acc222b0d3006e51101331e532e24081e2f08a2 in C:\openjdk-20 
# Thu, 20 Oct 2022 20:21:17 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 20 Oct 2022 20:21:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5ead999142ecce15e02523c49706a633fa708374d94bb65a254e3a3c117d609b`  
		Size: 103.4 MB (103377244 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a6a667d76c19fca171390d60fb90c40e16c777050e943a7fe17ad7686841f0f`  
		Last Modified: Wed, 12 Oct 2022 16:02:59 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4315d417eb7958a05c7977d0ea6b1b4745e46725d02f23235173bbad2c73101d`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c783713d738fc9dfff161ad3ff4369333cd0881466ab886feb09e6ef3508512e`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05686fefb2145f84031cd9cae616dd90496d078df87f19c080931972eb700e7c`  
		Last Modified: Wed, 12 Oct 2022 16:53:09 GMT  
		Size: 67.2 KB (67186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab8462cae193737dba91e48900abf79d1b7234b48f337497ae0abfe9d8189e5`  
		Last Modified: Wed, 12 Oct 2022 16:53:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aac413d21efae6c790b43f7a0530f0b87ec29bbc05ecd3042c6dc4fe4d92701`  
		Last Modified: Thu, 20 Oct 2022 20:24:31 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec52f04473aaa7472c0e7765291775cb7fafc93711000d26f202a6ba9f6048a`  
		Last Modified: Thu, 20 Oct 2022 20:24:50 GMT  
		Size: 192.1 MB (192081592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6988eb64326cd55d7b5d8d1c9dbfab154ec489d7d63dbf7bdcc9fbe772f28001`  
		Last Modified: Thu, 20 Oct 2022 20:24:32 GMT  
		Size: 3.8 MB (3754930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7976cddd9c075fbd7d24e3244171f971400a7e2ae7e60bd733156b1cd9f3f47e`  
		Last Modified: Thu, 20 Oct 2022 20:24:31 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
