## `openjdk:8u292-jre-nanoserver`

```console
$ docker pull openjdk@sha256:53d11f58156a28b107fc81ae3e8674d2684f95c69fc2795f17e2d2d4fc0d7578
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `openjdk:8u292-jre-nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull openjdk@sha256:9eee906bf2f65dc0d3d6e3e55847c1f704913d1a067447578d821393aa7a6403
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139719076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d708d2f1be749c341d58dc35bf50bfee05381da5cfb152d952058ff0d2996332`
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
# Thu, 22 Apr 2021 08:44:31 GMT
COPY dir:f730d49fd573406c508c5c18daca9d2bf81afd7c16f0b64747f54fe283bbc615 in C:\openjdk-8 
# Thu, 22 Apr 2021 08:44:49 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:7ce0259c8d0fb0a01dcacd1acd61103f9f4a96b9235be5b53f42b2fb4135b2eb`  
		Last Modified: Thu, 22 Apr 2021 08:57:15 GMT  
		Size: 38.2 MB (38216847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b81b5594dac1b205e196ae1919c43bf080fe754006a647c1d6f68cd96bf700`  
		Last Modified: Thu, 22 Apr 2021 08:56:28 GMT  
		Size: 90.3 KB (90265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
