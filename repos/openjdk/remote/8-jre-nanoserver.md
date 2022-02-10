## `openjdk:8-jre-nanoserver`

```console
$ docker pull openjdk@sha256:f9c54f45d2ce94585c769baf4e2d8f853fbad48154884e0ef403f7737d4c9936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `openjdk:8-jre-nanoserver` - windows version 10.0.17763.2565; amd64

```console
$ docker pull openjdk@sha256:19fba98d836be1c3db780975124e1775896b8b1a1093897db27f8e6640321df8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141478977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d23db030b3916722e1bcc0a3010048e829c271deb7a83f3d12515fedd330d7e`
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
# Wed, 09 Feb 2022 19:13:18 GMT
COPY dir:f4c77e4259f68c5f890bc7ab442034fb0a5366735393f4c5400d26f276285797 in C:\openjdk-8 
# Wed, 09 Feb 2022 19:13:34 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:e25b9fa0c40d2ec111c5b023f20463af736155981034ab01bf4ab630bb6aa8dd`  
		Last Modified: Wed, 09 Feb 2022 19:35:57 GMT  
		Size: 38.3 MB (38264497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49aea2bbe677ca47c1122d7eed54608de2131c14b7336e71bcca96260eb4a242`  
		Last Modified: Wed, 09 Feb 2022 19:35:51 GMT  
		Size: 46.1 KB (46134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
