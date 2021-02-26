## `openjdk:17-ea-11-nanoserver`

```console
$ docker pull openjdk@sha256:8435e52e4639beae91e137af59cd366a007b4e373ecd03b7c4027105e7e69df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1757; amd64

### `openjdk:17-ea-11-nanoserver` - windows version 10.0.17763.1757; amd64

```console
$ docker pull openjdk@sha256:c289848e14abb106c11874d55f9b52acb1edd6f9d6434bd2784855c826a4b9ce
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.2 MB (286226677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfe04d40b060a0112b54bfcdab5fa14918bcb4dfc89b3f7014578629ca844df5`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 02 Feb 2021 13:06:30 GMT
RUN Apply image 1809-amd64
# Wed, 10 Feb 2021 16:45:48 GMT
SHELL [cmd /s /c]
# Wed, 10 Feb 2021 16:45:49 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 10 Feb 2021 16:45:49 GMT
USER ContainerAdministrator
# Wed, 10 Feb 2021 16:46:03 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 10 Feb 2021 16:46:04 GMT
USER ContainerUser
# Fri, 26 Feb 2021 21:19:07 GMT
ENV JAVA_VERSION=17-ea+11
# Fri, 26 Feb 2021 21:19:27 GMT
COPY dir:4637f9cc17d2a77f74e25be79b0bb582010260f23630a059676a6cd8c917d07d in C:\openjdk-17 
# Fri, 26 Feb 2021 21:19:52 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 26 Feb 2021 21:19:53 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ba17af31b9276ee11fdf859681b442db50979a39eff4cea2a559a5755cedbe01`  
		Size: 101.4 MB (101406193 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:89effbaeeb74323a670701c3b9dac248927e603ffb2d7efed14d993d32f7c183`  
		Last Modified: Wed, 10 Feb 2021 17:17:35 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba245c3ca8dc95a5fefadb2d7b2366434552cc96ad3951f7028404924978fe3`  
		Last Modified: Wed, 10 Feb 2021 17:17:35 GMT  
		Size: 1.1 KB (1085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1331b1edc6cf93ddcbfd0ea0179ca55d1bc1fd44fee36a6d4260248d6207a6`  
		Last Modified: Wed, 10 Feb 2021 17:17:35 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ea90039b4b8e858352f401598e9a3aab5416bb5c88d71cc86d8cd325fe8586`  
		Last Modified: Wed, 10 Feb 2021 17:17:34 GMT  
		Size: 68.2 KB (68240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612927d1022d536248e669e8c4abbee53b84db28247493cf7238816707bc0e1e`  
		Last Modified: Wed, 10 Feb 2021 17:17:32 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdc33fce42777b8b96f516d9611e73509303aacc45acf20965141c905623ba8`  
		Last Modified: Fri, 26 Feb 2021 21:30:52 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d435599268f8c6e09740daf6545adf370604c3657a20467def3f0f02efb28d3`  
		Last Modified: Fri, 26 Feb 2021 21:31:11 GMT  
		Size: 181.1 MB (181068607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9554be58aafa361b62d98c226c6a258f5563c3092c4e928d4acbc1148c0ace2e`  
		Last Modified: Fri, 26 Feb 2021 21:30:53 GMT  
		Size: 3.7 MB (3676878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36b3c7799c645ef09174a3d24b8499fb8201dcda092bb70e295999ecd1aa6ba`  
		Last Modified: Fri, 26 Feb 2021 21:30:52 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
