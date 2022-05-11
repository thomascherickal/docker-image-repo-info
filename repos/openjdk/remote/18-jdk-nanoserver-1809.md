## `openjdk:18-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:26dfedcd04a70680027fcd49932ceb2077e6d037f2ea4b584ded92ad15e494ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `openjdk:18-jdk-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull openjdk@sha256:2997748b942a0f2d5c164824062ffb0d1137049b698a26a92dbd2b386328f082
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.0 MB (291019867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36870dc5fa75f95449e678030764e489ad7236b6aabec35a996d8ad29714a635`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:49:49 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:38:25 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:38:26 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:38:34 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 11 May 2022 15:38:35 GMT
USER ContainerUser
# Wed, 11 May 2022 15:38:35 GMT
ENV JAVA_VERSION=18.0.1.1
# Wed, 11 May 2022 15:38:51 GMT
COPY dir:73b3cefd3226759501d1f46bed25bbfcfd2faba5ebc2541b7c4b8c54b01cceae in C:\openjdk-18 
# Wed, 11 May 2022 15:39:08 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 11 May 2022 15:39:09 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5592374182790eb41396d922d16be86f39a125562f29ea3ed221a94aeec2af45`  
		Last Modified: Wed, 11 May 2022 16:00:35 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe0a635f4712b91afa413318e0a948aaa1527a0abd4203e081072e463b8177a`  
		Last Modified: Wed, 11 May 2022 16:11:41 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2704501ef828911abed0544bb540021597f796708fd7891256f5f522aabd665d`  
		Last Modified: Wed, 11 May 2022 16:11:41 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2326fce13e090e04749126c3f5d8727382eb4d27189ae964e837084931175e5`  
		Last Modified: Wed, 11 May 2022 16:11:41 GMT  
		Size: 70.2 KB (70162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80f63e6917ef6009d30cbaec20c47b3630c01367519be8f448aa393f737d0d1`  
		Last Modified: Wed, 11 May 2022 16:11:38 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f650ac6065138cf0fca7a3fa39f2428de16565f26c9093e8bb40eac0e0ab4792`  
		Last Modified: Wed, 11 May 2022 16:11:38 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a69a9df5bad4841a8f82e2aa73a51f1494fa93b7bd17f0afff9a6fb393295b`  
		Last Modified: Wed, 11 May 2022 16:15:10 GMT  
		Size: 184.2 MB (184223367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bd1b0b37144fe0ab8738d4aacadcb84e526617f34396bac9d871b5fc9d4a08`  
		Last Modified: Wed, 11 May 2022 16:11:39 GMT  
		Size: 3.6 MB (3586013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b443b6c99e9222ed26eb2135d7b13f3de6451f72ab794d4f1bd6e6b916bb9443`  
		Last Modified: Wed, 11 May 2022 16:11:38 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
