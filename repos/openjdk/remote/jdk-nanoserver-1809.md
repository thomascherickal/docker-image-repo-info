## `openjdk:jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c02cc2a68ee13393dc47419e1b507e78ddf00158f068f0f36e37f343f7ad70d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:jdk-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:61063cb92f412e507c269b7ca335f25640507058240c6bf39f43c278e4b1c33e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.4 MB (298406099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6254dba2b2962a1d712e3ea2afba924ffa760d66d4c6a278cf1afcffbf01e0`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:12:39 GMT
ENV JAVA_HOME=C:\openjdk-14
# Wed, 15 Jul 2020 02:12:39 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 02:12:50 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 02:12:51 GMT
USER ContainerUser
# Wed, 15 Jul 2020 02:12:52 GMT
ENV JAVA_VERSION=14.0.2
# Wed, 15 Jul 2020 02:13:42 GMT
COPY dir:3af480213c50f048b93f5646f49ddcfa051042f65b9b399de73d2b228bd2576f in C:\openjdk-14 
# Wed, 15 Jul 2020 02:13:59 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 15 Jul 2020 02:14:00 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d3e6cef870db96286acadd1f120ec81c36417ee6a78d10f6fc2f8c22a2cc75`  
		Last Modified: Wed, 15 Jul 2020 02:48:53 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9395c647ca5e721143135d323ee31b938bb8873a7a95682f423118071b7262a3`  
		Last Modified: Wed, 15 Jul 2020 02:48:52 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29f79e1f4e65675159a1d1ce6fe8b4b5365451a422de83abe78e7773ec31c27`  
		Last Modified: Wed, 15 Jul 2020 02:48:52 GMT  
		Size: 68.6 KB (68639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d66f747adef6987210bf83049f9d4d1dd2df5258cf8f0a7173bd1f06e5727a`  
		Last Modified: Wed, 15 Jul 2020 02:48:50 GMT  
		Size: 907.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7463addf7a99138a5d8c46c54d63b3862928c621aa8a4d9a478e50b52866d99`  
		Last Modified: Wed, 15 Jul 2020 02:48:50 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dac2fc58b2c72bc9d2dd844c2bd6d71912ed8f8f6eadbad0a46edafc88ff8059`  
		Last Modified: Wed, 15 Jul 2020 02:49:11 GMT  
		Size: 194.0 MB (193968614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf7e0241166b58b1c70afc2b3707b6476c9fe62b2d2f8f3f5880159a1b3771c`  
		Last Modified: Wed, 15 Jul 2020 02:48:51 GMT  
		Size: 3.5 MB (3467918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e382f43173560e3eb774a1cc53beb80e9b6f57ed86faabaf6fd2ccbba7e2ae3a`  
		Last Modified: Wed, 15 Jul 2020 02:48:50 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
