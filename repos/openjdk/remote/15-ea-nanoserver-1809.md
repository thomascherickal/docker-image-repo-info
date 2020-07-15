## `openjdk:15-ea-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c2d09fd9b77c9e1197097833c93aed16b616c1723fa6ab53c585ac1a4e97c50d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:15-ea-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:2670ab2873f715034c52b06f863c91ecaa5959b520b130457dadcaa9ee1f4a3a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295784133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a733a0521336cc0c7c5819824b1642704f5244d4c27ede08bf1a9f2408ef9f7b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:03:33 GMT
ENV JAVA_HOME=C:\openjdk-15
# Wed, 15 Jul 2020 02:03:34 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 02:03:45 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 02:03:45 GMT
USER ContainerUser
# Wed, 15 Jul 2020 02:03:46 GMT
ENV JAVA_VERSION=15-ea+31
# Wed, 15 Jul 2020 02:04:35 GMT
COPY dir:8c9ba2918e3c2737605432ccf9b34e043f1efb82354836eddf5cf3bbad167ed1 in C:\openjdk-15 
# Wed, 15 Jul 2020 02:04:56 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Wed, 15 Jul 2020 02:04:57 GMT
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
	-	`sha256:c17195adca743b283e9fdf01c1670d33e88c1b7f8ad0ff6a19afa11f90abbdaa`  
		Last Modified: Wed, 15 Jul 2020 02:46:29 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d4978cbb8680255360d757c7d46e5a1c7c246047f93257964335958cd1b1307`  
		Last Modified: Wed, 15 Jul 2020 02:46:30 GMT  
		Size: 886.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a772f899b85a5ec3b1356709ac25974f0b40a2729a3b6bd12f56e44a5cee769d`  
		Last Modified: Wed, 15 Jul 2020 02:46:29 GMT  
		Size: 67.3 KB (67317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29415bb95c60f5fdec327237a6683b4a710b6cf5925d41adef8d21f8a277140e`  
		Last Modified: Wed, 15 Jul 2020 02:46:26 GMT  
		Size: 870.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4d167374c1f267fa41199abc5780b1f04a8fc90a6c69938a87eebe4c245577`  
		Last Modified: Wed, 15 Jul 2020 02:46:25 GMT  
		Size: 865.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5f432d24c458428def33fc42cc687b0fae9090747d863f5008924c4be74752`  
		Last Modified: Wed, 15 Jul 2020 02:46:45 GMT  
		Size: 191.3 MB (191332853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1753d21d74f5ffb0194bddeda9bfccb5d9dba2263950491773b2e49a1d8c3a46`  
		Last Modified: Wed, 15 Jul 2020 02:46:26 GMT  
		Size: 3.5 MB (3483052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba18cfcbc125b589ddb665c41a673e9cbfeafce350fbd29ab94198f15e46ba`  
		Last Modified: Wed, 15 Jul 2020 02:46:26 GMT  
		Size: 914.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
