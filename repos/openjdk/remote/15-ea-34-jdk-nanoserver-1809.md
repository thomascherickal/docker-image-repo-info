## `openjdk:15-ea-34-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:78646624ea09d35fedf797a0203a0506ad7b7f5f9b9162b6491dd7bf93e14068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:15-ea-34-jdk-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:df3e735ea4d2f38c6831edfa237044075bbd323f6716e5b25c60fa52b35850a0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295809906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:573e529d1134df13cec4281ed10baaaa98295d432e9a71858197ad5bd51f9abe`
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
# Fri, 24 Jul 2020 18:27:57 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Fri, 24 Jul 2020 18:27:58 GMT
USER ContainerUser
# Fri, 31 Jul 2020 22:28:28 GMT
ENV JAVA_VERSION=15-ea+34
# Fri, 31 Jul 2020 22:29:15 GMT
COPY dir:eb796afe2a0f9fd8cac7eb8e3ee7cf012bc55673735debd6f40a52cb08220863 in C:\openjdk-15 
# Fri, 31 Jul 2020 22:29:33 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Fri, 31 Jul 2020 22:29:35 GMT
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
	-	`sha256:ff0cf1f70e8582e4556e8be6e96025ad2d6e372cf6fdaaffb1cda64b76d8150f`  
		Last Modified: Fri, 24 Jul 2020 18:36:57 GMT  
		Size: 69.4 KB (69424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60b2e2d468204c429e90685f0b28fc4a0bcb8c1b50ce01d726ca37b23d8a576`  
		Last Modified: Fri, 24 Jul 2020 18:36:54 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc73af37291c976473ad3e0d2e5532b1acc0809648ab3b7fbc415e0973c1189e`  
		Last Modified: Fri, 31 Jul 2020 22:50:04 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17175188565b3fd96716dfa451e67e1d52e8af1fec0ca45882ffe8606add9fb6`  
		Last Modified: Fri, 31 Jul 2020 22:50:42 GMT  
		Size: 191.4 MB (191355471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b95e683e34a66fb93e477d8d9b0f22becabf7ba02220a18752757f69507633`  
		Last Modified: Fri, 31 Jul 2020 22:50:08 GMT  
		Size: 3.5 MB (3484042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0a765b856005ef73509cec219ac285cf9756f01680210d261f15faefc8a5a3`  
		Last Modified: Fri, 31 Jul 2020 22:50:04 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
