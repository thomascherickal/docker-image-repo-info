## `openjdk:18-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:f1d0a518e0b7ca1e74bebfb5f3d893bddc4456ee7bdd516dbdbc4689c366483a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `openjdk:18-jdk-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull openjdk@sha256:7a61951ae96d5736907aff6888055362ba5fb0db490bb8ea4c8607cdc0d71323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.4 MB (289350475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b4c14a3d2efdfcdac52e66a1418def5cf203e60e1acef3fd03dd2c37876b42b`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 18:17:55 GMT
SHELL [cmd /s /c]
# Thu, 14 Oct 2021 00:38:45 GMT
ENV JAVA_HOME=C:\openjdk-18
# Thu, 14 Oct 2021 00:38:45 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 00:38:59 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Thu, 14 Oct 2021 00:38:59 GMT
USER ContainerUser
# Sat, 16 Oct 2021 00:30:31 GMT
ENV JAVA_VERSION=18-ea+19
# Sat, 16 Oct 2021 00:30:46 GMT
COPY dir:2d0582dbad17d1ae6107202d52b0d3c503b000da22f128140d73fea211ca33c0 in C:\openjdk-18 
# Sat, 16 Oct 2021 00:31:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 16 Oct 2021 00:31:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ceff24c3c0c2c360cd3788fcde5c41e1d6601339f4944623c732558a6030e631`  
		Last Modified: Wed, 13 Oct 2021 19:12:58 GMT  
		Size: 1.1 KB (1058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11210a1a14144795863cc9df7368535adbfcea9f756732c5757ce09ae1126ff9`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef4f8f1bc44cf5deaf0e09239eb5f99652025d58114cc36025894b724e1e593`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528cd68420af607e2ba2867ba7f9e41b2412cc5fcd6ad946de4355966a18b56b`  
		Last Modified: Sat, 16 Oct 2021 00:39:37 GMT  
		Size: 71.6 KB (71641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee7149c120a9a849ece2e9be315293f5b77a4443d8f1cc13b6d4745290851a9`  
		Last Modified: Sat, 16 Oct 2021 00:39:34 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe9a148c867d39a74e17fc2363af94fcbc4c2103cce4319cd8ada2a1e336e60`  
		Last Modified: Sat, 16 Oct 2021 00:39:35 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bdd605ce3ca33fd2d2840837d450b93ee25e2c614a96f03ec68ed32e7fe483`  
		Last Modified: Sat, 16 Oct 2021 00:39:53 GMT  
		Size: 183.1 MB (183084695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2959835919831ba8a7f3cbca00e4aac9e15ef402d21e58309f259cc8ecade07`  
		Last Modified: Sat, 16 Oct 2021 00:39:35 GMT  
		Size: 3.5 MB (3525972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7fef5eda003d3c71b294bdbb4567db66eed3ac9906e0c7affd5418d26d3171`  
		Last Modified: Sat, 16 Oct 2021 00:39:34 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
