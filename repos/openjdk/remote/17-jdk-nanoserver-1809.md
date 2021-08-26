## `openjdk:17-jdk-nanoserver-1809`

```console
$ docker pull openjdk@sha256:2d372975dd191a4df79b87e36cff80f5228d4d5541ff46c44d33b8330c157468
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:17-jdk-nanoserver-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:39e52bd30a40eee3dfc7d1ad6251749c935bb1ec4447a490e3829431bb59ad02
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.6 MB (288561335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e6efc2e5d90b9c4c8be7232fe37d359c446d2fb3833270880e3c061d4f3c0f`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:34:07 GMT
SHELL [cmd /s /c]
# Wed, 25 Aug 2021 17:12:27 GMT
ENV JAVA_HOME=C:\openjdk-17
# Wed, 25 Aug 2021 17:12:28 GMT
USER ContainerAdministrator
# Wed, 25 Aug 2021 17:12:36 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 25 Aug 2021 17:12:37 GMT
USER ContainerUser
# Wed, 25 Aug 2021 17:12:38 GMT
ENV JAVA_VERSION=17
# Wed, 25 Aug 2021 17:12:53 GMT
COPY dir:16139fd5761a261a0505c9fb2561cbcbf9614d8d2403d5d2b56478bd7a396d2c in C:\openjdk-17 
# Wed, 25 Aug 2021 17:13:06 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Wed, 25 Aug 2021 17:13:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9191bd6656c8ea186f621f667fb09a30387fae304b3e7817fd7e8258c022d185`  
		Last Modified: Wed, 25 Aug 2021 23:21:14 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb61684a1f9640010a62f8d5b1e0b99f82c722a9fb2b27637f7224d6e185363`  
		Last Modified: Thu, 26 Aug 2021 00:41:35 GMT  
		Size: 1.1 KB (1062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914defc1dc7ce0b2a6d142c614b8452d213160de268d1997faceca020eb7fac1`  
		Last Modified: Thu, 26 Aug 2021 00:41:35 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd9a55bef3e0a545dbacd3e4311112cff54fb77e31345690cbea44f8e5c0d31`  
		Last Modified: Thu, 26 Aug 2021 00:41:35 GMT  
		Size: 69.1 KB (69093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb599492704cad40508ac36c996f14767be49bfd699adc2f8117bcdad3477bc4`  
		Last Modified: Thu, 26 Aug 2021 00:41:31 GMT  
		Size: 1.1 KB (1050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e27af53895a8de0f422d8217a5d87aef6030597380382bb8a881cb561282f1`  
		Last Modified: Thu, 26 Aug 2021 00:41:31 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004bdc97f34a181f328024563621b8e7e26775878be4e054000c83c2816d8b3`  
		Last Modified: Thu, 26 Aug 2021 00:41:53 GMT  
		Size: 182.1 MB (182098571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422bcba395df1e74e2675d0f310cf6c1e0a3c2f28b840e5313a31db56e2a746`  
		Last Modified: Thu, 26 Aug 2021 00:41:36 GMT  
		Size: 3.6 MB (3646180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caa46c22e1ac359d206cbad718807daaaa6e6ec6173bcfd4cff5cde8d346d1f`  
		Last Modified: Thu, 26 Aug 2021 00:41:32 GMT  
		Size: 1.1 KB (1057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
