## `openjdk:18-ea-jdk-nanoserver`

```console
$ docker pull openjdk@sha256:f726a736c8869eecedd4d4d3fae6ab586f1d32786a5f1493b337f647f33bdd55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:18-ea-jdk-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:6b794a8078022362801779a17dc7976dde708cf523287610f017209f914c6b03
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.5 MB (290461529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:169afbb83f26c40e26f05acfb3e25d970af46bd51a0564fc74ee4a61050cdbe8`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 05:18:44 GMT
SHELL [cmd /s /c]
# Sat, 18 Dec 2021 07:11:41 GMT
ENV JAVA_HOME=C:\openjdk-18
# Sat, 18 Dec 2021 07:11:42 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 07:11:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 18 Dec 2021 07:11:54 GMT
USER ContainerUser
# Sat, 18 Dec 2021 07:11:54 GMT
ENV JAVA_VERSION=18-ea+28
# Sat, 18 Dec 2021 07:12:11 GMT
COPY dir:ab4ea4e60bba1acab093f8402740745f17f8a43a4c0eb64669009e3cf65835b1 in C:\openjdk-18 
# Sat, 18 Dec 2021 07:12:25 GMT
RUN echo Verifying install ... 	&& echo   javac --version && javac --version 	&& echo   java --version && java --version 	&& echo Complete.
# Sat, 18 Dec 2021 07:12:26 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4c557aac927613dd487d7c04b01a8eeb8ad174693f61b14c8f4285f1db6afdd2`  
		Last Modified: Sat, 18 Dec 2021 06:13:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb09a08117aed517f83acd09c46245354fda9e1f94c432b6c5be4758bd11846a`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9558b80b57be79d231423f31ff119a52bfde5373d41866669b3536cad1fe939`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f711c3cc04e41a513139b9dce135ea0dc407bb92c80b5fb14341e73eca8e7`  
		Last Modified: Sat, 18 Dec 2021 11:08:07 GMT  
		Size: 67.3 KB (67275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8203006c00a339abd7dace4c1b632bcbb99479c9cbd36cdf65f5ca4363d6872d`  
		Last Modified: Sat, 18 Dec 2021 11:08:05 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92c56341bc37aeb9dced1a790aabfb857264a683ff87efdabda7cde20153cb3`  
		Last Modified: Sat, 18 Dec 2021 11:08:04 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a0eeec6c65b5da356164d03a8b1548b609259af323b7580860535264b4d116`  
		Last Modified: Sat, 18 Dec 2021 11:11:27 GMT  
		Size: 183.9 MB (183935523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe2b5f2344c7a928cf967a21fa3e5352e527626aeb89afc7efeefbcfeda3ed2`  
		Last Modified: Sat, 18 Dec 2021 11:08:06 GMT  
		Size: 3.5 MB (3547760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5e3b78c6f9611cc516b4cccddb45d4654e69f04ed43bedde4a904526a0ba66`  
		Last Modified: Sat, 18 Dec 2021 11:08:04 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
