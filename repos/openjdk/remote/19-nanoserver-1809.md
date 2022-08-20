## `openjdk:19-nanoserver-1809`

```console
$ docker pull openjdk@sha256:afc9376bf03008ddf971fc6560502cba8f8a3fb64c9e1e608f32bec2ee0195bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `openjdk:19-nanoserver-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull openjdk@sha256:c22bd57957abda7f7f228fb3c737ecc4d50caeb22a80b128986e2a16f5007057
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.2 MB (298211835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f221d7c9371ebccce1bfe0b7c199487cf700f2805ba452663145e169c70f64c`
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
# Sat, 20 Aug 2022 01:59:46 GMT
ENV JAVA_VERSION=19
# Sat, 20 Aug 2022 02:00:01 GMT
COPY dir:ad572564354aac78397e790af4fedd1886f683bcb0c086fecfa550483cfa75ad in C:\openjdk-19 
# Sat, 20 Aug 2022 02:00:17 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 20 Aug 2022 02:00:18 GMT
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
	-	`sha256:e89fffe5ac39cacb4f19907b85adcd7bbbbaa1d15b72e9972c5e1ee1875ae27f`  
		Last Modified: Sat, 20 Aug 2022 02:08:55 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27fc1d765614dbbe3fbd6f6b48b25d0577c85213c2c6f7268fe661587550443`  
		Last Modified: Sat, 20 Aug 2022 02:09:16 GMT  
		Size: 191.2 MB (191222742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc11711bf63c3a391808bca4c5a13642057c950a1fd0f2426ddc4432c5fd6aea`  
		Last Modified: Sat, 20 Aug 2022 02:08:56 GMT  
		Size: 3.7 MB (3709663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c129f14d9bb484da5e16782520f42407ef658acd6ba1784068cab99ca8bdb7`  
		Last Modified: Sat, 20 Aug 2022 02:08:55 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
