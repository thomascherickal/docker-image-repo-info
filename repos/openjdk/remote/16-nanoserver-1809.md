## `openjdk:16-nanoserver-1809`

```console
$ docker pull openjdk@sha256:5dcb57e7b0692d3cd0289138f2820f48e38b4c952baeadeb8c7db3e629bfcc8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:16-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:5f1aee39dfb7a63f0ec6fe167701d0ce080c35524c37b5720a103c2a6ec93789
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.7 MB (296656321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49198f624a77c16af681b9322e5f3435158ff9738a29f1e715a4602bdb34443`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 01:54:44 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 15 Jul 2020 01:54:45 GMT
USER ContainerAdministrator
# Fri, 24 Jul 2020 18:21:01 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Fri, 24 Jul 2020 18:21:02 GMT
USER ContainerUser
# Fri, 31 Jul 2020 22:21:13 GMT
ENV JAVA_VERSION=16-ea+8
# Fri, 31 Jul 2020 22:21:59 GMT
COPY dir:4a1a62c875e9e13d011d30c58f33306ef04c8b5c21f1203cb870721cab4a1792 in C:\openjdk-16 
# Fri, 31 Jul 2020 22:22:35 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 31 Jul 2020 22:22:36 GMT
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
	-	`sha256:952f154db0b1aa57586a649f933acc22620a18dc11bfe0f2369af17af77fd616`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d574471402fee7c0d2fb574eb4bbfd848f720c971dc4d9318a7437da54d1ee`  
		Last Modified: Wed, 15 Jul 2020 02:43:54 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa94d52ff38f89a9e35647ee58e1b9d5c1ee9f238d17d1d94d294263683a8fc7`  
		Last Modified: Fri, 24 Jul 2020 18:34:41 GMT  
		Size: 65.3 KB (65316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70146e6967d5a15f9a4884bb2688dbc7af97e64172e951cc00ccbe779da256fe`  
		Last Modified: Fri, 24 Jul 2020 18:34:38 GMT  
		Size: 822.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b9632a3d3924fa19803b3c627b969dd464a3aed5ac80ec30adeb6b3ea36f8b`  
		Last Modified: Fri, 31 Jul 2020 22:38:29 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd2ec333317188f85fa5a53345d8c370369dc58f41b1a03bdc116464f2c6c5f`  
		Last Modified: Fri, 31 Jul 2020 22:41:54 GMT  
		Size: 192.2 MB (192170995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b8d868190a85b1ba9b693804144c55856a1d7ebe53c4874d3f12a03053c769`  
		Last Modified: Fri, 31 Jul 2020 22:38:33 GMT  
		Size: 3.5 MB (3519148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279eb507078322b12dc57f54c2e31a1ea55e9467e9c2a99e4cb6dc0532881b6`  
		Last Modified: Fri, 31 Jul 2020 22:38:29 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
