## `openjdk:15-ea-nanoserver`

```console
$ docker pull openjdk@sha256:3d553c878ad8d2e0842f0777f6b4725a5fec5ac8b98c8538c31ebe3d925cfd60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `openjdk:15-ea-nanoserver` - windows version 10.0.17763.1158; amd64

```console
$ docker pull openjdk@sha256:2fec4392cf25ff1e9a090c8020cb401464c235b58c9b5d173564e6235a141a91
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.7 MB (296652930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad027a4d5432b8423b4cb975d5a81dbd0d30fd0253e586b779faa3deaae9c65`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Tue, 14 Apr 2020 21:42:38 GMT
SHELL [cmd /s /c]
# Tue, 14 Apr 2020 21:42:39 GMT
ENV JAVA_HOME=C:\openjdk-15
# Tue, 14 Apr 2020 21:42:39 GMT
USER ContainerAdministrator
# Tue, 14 Apr 2020 21:42:54 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Tue, 14 Apr 2020 21:42:54 GMT
USER ContainerUser
# Tue, 14 Apr 2020 21:42:55 GMT
ENV JAVA_VERSION=15-ea+18
# Tue, 14 Apr 2020 21:43:40 GMT
COPY dir:4b0099682e8b4a04796ff18349ecd4655059bff1caaf3119e2b54efe2598d1ef in C:\openjdk-15 
# Tue, 14 Apr 2020 21:43:58 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version
# Tue, 14 Apr 2020 21:43:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:895ca47ba9cf1a5b61a0721217cfcc038bbe9a4987c7536321c3ac51ef8e5e0c`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bcf297e34b7d011805160436d6acaba77887d05e2acd81e88acd84ad22cdff1`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 830.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9641626825020cd19b05bbf1f20b92df3d267d2aade5a84deef0163b791a895b`  
		Last Modified: Tue, 14 Apr 2020 22:17:22 GMT  
		Size: 819.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062e1c072d6c921a1b4e4db61fa592b7f9ccbc231f6c5cc8dfd4417fc317438c`  
		Last Modified: Tue, 14 Apr 2020 22:17:21 GMT  
		Size: 67.0 KB (67045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe221d18f1e3ca2b86519debf76a76b4ba0e95f42490a1a161bffea2d3306309`  
		Last Modified: Tue, 14 Apr 2020 22:17:19 GMT  
		Size: 824.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe3e3125eed648c6dda1efd58cff641a62875da887d52bcf1f9384ce0dcae86`  
		Last Modified: Tue, 14 Apr 2020 22:17:19 GMT  
		Size: 832.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59919e3e4cd4626905df4e5457daf80ec43de8feabfc28b255f9717276d2fe60`  
		Last Modified: Tue, 14 Apr 2020 22:17:37 GMT  
		Size: 192.0 MB (192001620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1e469d04944c91a623acd88ff2104a2c96cf89e503ea5153c95b9fd553b61d`  
		Last Modified: Tue, 14 Apr 2020 22:17:19 GMT  
		Size: 3.5 MB (3460910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f553010ae60952d0f250ff0dd8e9a0f65b1e490aa0bfbcfc151f7cabc464ee65`  
		Last Modified: Tue, 14 Apr 2020 22:17:19 GMT  
		Size: 837.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
