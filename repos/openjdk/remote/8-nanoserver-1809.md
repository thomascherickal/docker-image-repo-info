## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:67b0fca4a4ac6df3b8e76527040a11e5d154ff1f1cab8f8496e5b7ebe83c24d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:5f35a08a7b977ece9794974cde8d4f9b20f7445073529c221f6c09dabfdf2919
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202553875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c909cff7f6eb761852b8729076a3f773aeb33e319aa19e9c816ad835bd9a9d27`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:53:40 GMT
SHELL [cmd /s /c]
# Wed, 14 Apr 2021 17:27:30 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 14 Apr 2021 17:27:31 GMT
USER ContainerAdministrator
# Wed, 14 Apr 2021 17:27:45 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 14 Apr 2021 17:27:45 GMT
USER ContainerUser
# Thu, 22 Apr 2021 08:30:25 GMT
ENV JAVA_VERSION=8u292
# Thu, 22 Apr 2021 08:30:40 GMT
COPY dir:04533fde1b9ea0cd60bd0fd48d2f644dab91f29f3b0d8a376770cc16b38c53d2 in C:\openjdk-8 
# Thu, 22 Apr 2021 08:30:57 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c2c727299531adc7c2aacb1f062d72fd42cec96a0d235b3e5b0afe03e9ddbc7d`  
		Last Modified: Wed, 14 Apr 2021 17:41:13 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c7d921929195146d6442e27a405dc06676d7e52a8806c1041a8a821b3ae91d`  
		Last Modified: Wed, 14 Apr 2021 17:54:28 GMT  
		Size: 1.0 KB (1041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17b71c3462fefa5234492d0bc83528577a7de4432da7075bee4accc63546d8`  
		Last Modified: Wed, 14 Apr 2021 17:54:27 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a3200fb343c477ec4976a94e9ad98dee760d79fc21d4bfc39becf564ff377a`  
		Last Modified: Wed, 14 Apr 2021 17:54:25 GMT  
		Size: 66.2 KB (66240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84869171477acabf60cdc0f43e92b340759190808d1e93844a909b9f45d2062`  
		Last Modified: Wed, 14 Apr 2021 17:54:25 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232f793e66b108c5429bc49c856b09452a12e8b500ea8cb9495a3a89cee70c9c`  
		Last Modified: Thu, 22 Apr 2021 08:55:37 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dee5e4779b38d988d1e51f75398ca79365abbab00e68263d019d97fcb2a4dc7`  
		Last Modified: Thu, 22 Apr 2021 08:55:52 GMT  
		Size: 101.0 MB (101039439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b279d3a76c9175ffa19a458573058b02b887e0f15e92d5c612e2314856ca815a`  
		Last Modified: Thu, 22 Apr 2021 08:55:37 GMT  
		Size: 102.5 KB (102472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
