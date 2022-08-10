## `openjdk:19-nanoserver-1809`

```console
$ docker pull openjdk@sha256:87c9480424fbe114f5fac5ddfcf5a0719d8106604cd3e70c4ffdc0b7633034fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:19-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:5379eaf27f86cf63dc406b1bb306d55af1a09c9fb1deabdfa06c31f42f1fe7ff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298184679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda251cb152b1500e9a60ad0e678442648c265b7a76f8c8e112b606511d7fae5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:57:07 GMT
SHELL [cmd /s /c]
# Wed, 10 Aug 2022 17:04:59 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 10 Aug 2022 17:05:00 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 17:05:08 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Aug 2022 17:05:08 GMT
USER ContainerUser
# Wed, 10 Aug 2022 17:05:09 GMT
ENV JAVA_VERSION=19-ea+34
# Wed, 10 Aug 2022 17:05:24 GMT
COPY dir:a915abe9a325cfc0cb6f8cb6819a212af006cc12f498bc43c7ec9f4f4c627c43 in C:\openjdk-19 
# Wed, 10 Aug 2022 17:05:38 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 10 Aug 2022 17:05:39 GMT
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
	-	`sha256:0913a46926bf2c3f8990a8106449896cd6928beac2cf27f0dcd12a550a8ad44f`  
		Last Modified: Wed, 10 Aug 2022 17:30:44 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a690411fd73885d611135412ef0415c71c59a51a6425b5c46f09baa5e433afca`  
		Last Modified: Wed, 10 Aug 2022 17:30:44 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fd9039faf6dfc9d95d9c9eba070a57322959390e85c5df2ab02a10d61886f0`  
		Last Modified: Wed, 10 Aug 2022 17:30:44 GMT  
		Size: 68.4 KB (68428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a525dcc9920c1f15f2c65091b9156b9520fdf19c488340cf6edacf8a201be4`  
		Last Modified: Wed, 10 Aug 2022 17:30:42 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fceba647b7b97021c4a54fff6fa30536e38a376165311f4c68226b4363e586`  
		Last Modified: Wed, 10 Aug 2022 17:30:42 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba45ae5b5cee5794f86ba251266e4d9263c828fe860d27e52ebcec8d3eedfa1`  
		Last Modified: Wed, 10 Aug 2022 17:31:02 GMT  
		Size: 191.2 MB (191187267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c173b7565f58f5802c34ef377024989f1d8013d41f96abfa4dbc1c15625184`  
		Last Modified: Wed, 10 Aug 2022 17:30:43 GMT  
		Size: 3.7 MB (3717861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486828e8c0a107340482279c781e048561f1d109fa4a19a02eee945058e15fd0`  
		Last Modified: Wed, 10 Aug 2022 17:30:42 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
