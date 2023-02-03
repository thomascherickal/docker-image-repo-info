## `openjdk:21-nanoserver-1809`

```console
$ docker pull openjdk@sha256:9dc5ccea72724a9babb98dfceef94ad8701ee2be8aa7c37df209de4cf2a7b968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `openjdk:21-nanoserver-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull openjdk@sha256:fda830ce2f7507108161bcfa074a9d496d8c6c5b6b38babe78cee718047491c6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.7 MB (304674730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb581403df294f030964a1ab6909dd1b89470c452ddc10d5feddb27f1d7520f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:45:31 GMT
SHELL [cmd /s /c]
# Thu, 12 Jan 2023 05:11:18 GMT
ENV JAVA_HOME=C:\openjdk-21
# Thu, 12 Jan 2023 05:11:19 GMT
USER ContainerAdministrator
# Thu, 12 Jan 2023 05:11:34 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 12 Jan 2023 05:11:35 GMT
USER ContainerUser
# Thu, 02 Feb 2023 23:26:03 GMT
ENV JAVA_VERSION=21-ea+8
# Thu, 02 Feb 2023 23:26:21 GMT
COPY dir:8cd2df261fadf19c32e3a8626417a2129265e2a1e40fef8859f030df0642008b in C:\openjdk-21 
# Thu, 02 Feb 2023 23:26:56 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Thu, 02 Feb 2023 23:26:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea67a6bd980bdee35399883e5abcc31c738b338ad384b2f92d91a15cf09d9df`  
		Last Modified: Thu, 12 Jan 2023 02:40:16 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c10d054b2ffa414ee6a75be646bd3ee1ea6bd5a11e2400c757afeb68d8c6d4`  
		Last Modified: Thu, 12 Jan 2023 05:23:44 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e99b18c6e5f683aa5e6fa7ad7ce124fabae3b048287a183a71a7dc15df8ef6a`  
		Last Modified: Thu, 12 Jan 2023 05:23:44 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6700bb1c6480ee456d21843fdd01e9a05b05ea2d8ac6f54cbd75acbaafe6ab52`  
		Last Modified: Thu, 12 Jan 2023 05:23:44 GMT  
		Size: 69.3 KB (69271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9fc3250a046295f3386717ccc0548a5954c2c32fb3c4bbbc83dc8fdd13e1c27`  
		Last Modified: Thu, 12 Jan 2023 05:23:42 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9102bf959141256809e6966828620a02ee93ec22e9e2b4987b49f1b4370716b6`  
		Last Modified: Fri, 03 Feb 2023 00:25:03 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf9574f5be36713ef28395bf48c6e115950b145296ada3bcf91bba59825d40e`  
		Last Modified: Fri, 03 Feb 2023 00:25:26 GMT  
		Size: 194.1 MB (194117946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b354ab17c56262facf0ccc393bc22a57d1255a356444457527641a7523e93ce`  
		Last Modified: Fri, 03 Feb 2023 00:25:04 GMT  
		Size: 3.8 MB (3814507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acc462662328688f44df025043eabf8e9895fce0d5e09685655d6fccd353e1a`  
		Last Modified: Fri, 03 Feb 2023 00:25:03 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
