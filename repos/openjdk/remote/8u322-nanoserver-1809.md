## `openjdk:8u322-nanoserver-1809`

```console
$ docker pull openjdk@sha256:9e593eb9976265067f5375861e83050389ce56f718c4bece5f514bb2af77fc94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:8u322-nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:718246648dc9b402a02c3874f93425d1c8afbd0de309d1a3f6069960232a0888
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.3 MB (204306317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27cbc5c426a6584950a4e272c013e150bb95ddbdeade70097371cca7dff73536`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:45:32 GMT
SHELL [cmd /s /c]
# Wed, 09 Feb 2022 19:10:25 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 09 Feb 2022 19:10:26 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 19:10:34 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Feb 2022 19:10:34 GMT
USER ContainerUser
# Wed, 09 Feb 2022 19:10:35 GMT
ENV JAVA_VERSION=8u322
# Wed, 09 Feb 2022 19:10:58 GMT
COPY dir:70b73c62c79b1e3a83236c8add186d48955c92966a80012af2e52ff572318d7b in C:\openjdk-8 
# Wed, 09 Feb 2022 19:11:09 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5a7f567e84a5a148036156650a47ef7eec0187f17e880d3b475e51dacd70077b`  
		Last Modified: Wed, 09 Feb 2022 19:20:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cb9b26a104d74759a502b0c90a780aee0d761dfe3e9fb417d2007b3cb7d485`  
		Last Modified: Wed, 09 Feb 2022 19:34:57 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d4ba05dd1b8728630c569f843731260d412e4c9f030d420c1618480bcac501`  
		Last Modified: Wed, 09 Feb 2022 19:34:57 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e4c83b4a79fadb80d588586edabded16eb5e8825ebdb46060fbc1fa1f58db6`  
		Last Modified: Wed, 09 Feb 2022 19:34:54 GMT  
		Size: 75.5 KB (75468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b8b0b44ccb1496dbe415113fa78d4b15e1834e8a18db13d5dce829c44c957`  
		Last Modified: Wed, 09 Feb 2022 19:34:55 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a196df7f153311e927e2ab25ac1d4ffff4663c9abcc892718e2f3163933c58`  
		Last Modified: Wed, 09 Feb 2022 19:34:54 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b29a5ce102ec3b19ac94efe73869a0abc0288ccbbcf1b39a4363100731d1e85`  
		Last Modified: Wed, 09 Feb 2022 19:35:06 GMT  
		Size: 101.1 MB (101091452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8b3bd46c5095fff6b49972aa42fad9f66ecb8935ab0a9aa56b7a561f141b2f`  
		Last Modified: Wed, 09 Feb 2022 19:34:55 GMT  
		Size: 46.5 KB (46519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
