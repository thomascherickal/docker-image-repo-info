## `openjdk:19-nanoserver-1809`

```console
$ docker pull openjdk@sha256:984cbccd8bea08ad834ad0d031413a09aeeb6d5781d0100d4ee6bf5ff62af2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `openjdk:19-nanoserver-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull openjdk@sha256:285cd0e810ffc8d8997c53965c3ac50b7a761130385ce73abe54eef6d00831d8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295512925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5801146ab6337f2e20ec6a09d952855c6e6102853163a8bb398f277a237f21be`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 03 Mar 2022 14:36:26 GMT
RUN Apply image 1809-amd64
# Tue, 08 Mar 2022 21:56:20 GMT
SHELL [cmd /s /c]
# Wed, 09 Mar 2022 17:13:35 GMT
ENV JAVA_HOME=C:\openjdk-19
# Wed, 09 Mar 2022 17:13:36 GMT
USER ContainerAdministrator
# Wed, 09 Mar 2022 17:13:47 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Wed, 09 Mar 2022 17:13:48 GMT
USER ContainerUser
# Fri, 08 Apr 2022 20:19:18 GMT
ENV JAVA_VERSION=19-ea+17
# Fri, 08 Apr 2022 20:19:32 GMT
COPY dir:d0f49d250cc4c10e9825462746cd6078ddd77f0b59db92d6457b09a1aeb39bbd in C:\openjdk-19 
# Fri, 08 Apr 2022 20:20:02 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Fri, 08 Apr 2022 20:20:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e36e211379dc6a584a05a445fe37d396de6e76a42cc6742213c3cc3c656dd48`  
		Size: 103.1 MB (103054555 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e0065cd23a657c8f30ae5af121fd18451d2307835a1124ea57c80683eda26c94`  
		Last Modified: Tue, 08 Mar 2022 22:37:21 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab71e137ca33aa5127b0e55796dd1ffba9bdcf004bd9e37533e42daa5ebd2bf`  
		Last Modified: Wed, 09 Mar 2022 17:42:19 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b9123b1e06063521bbaeb5ac4dc7ac8960be154774560ca5c9db99a43b2d8d`  
		Last Modified: Wed, 09 Mar 2022 17:42:19 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ab23123853d0353a546935f5a1d10d91f5c5c44d79bf888ae0d353941c6938`  
		Last Modified: Wed, 09 Mar 2022 17:42:19 GMT  
		Size: 68.0 KB (68002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219e794e6ab490d19f1491c0d2de445c430aac5eceb51f362b916de14e9250d`  
		Last Modified: Wed, 09 Mar 2022 17:42:17 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29135c7cf99c8a5d9d59516ca5021a2fe004528ed396289915c56a27417a714d`  
		Last Modified: Fri, 08 Apr 2022 23:24:46 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39efc0156e7da051c353c5b72882eb58f707bd765d7464c26eb792a46039141`  
		Last Modified: Fri, 08 Apr 2022 23:25:04 GMT  
		Size: 188.8 MB (188800895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f169e105888309ea2ee4c8d5c1ea671660d3d73b588946fa70d22ce8ec1cec00`  
		Last Modified: Fri, 08 Apr 2022 23:24:47 GMT  
		Size: 3.6 MB (3582582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecada9818c5e8fbd782a844af0f523fcf9523d544f97feb2afff3d106f9afce5`  
		Last Modified: Fri, 08 Apr 2022 23:24:47 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
