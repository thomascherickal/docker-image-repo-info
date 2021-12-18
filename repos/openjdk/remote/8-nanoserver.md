## `openjdk:8-nanoserver`

```console
$ docker pull openjdk@sha256:a5bf926d0c683316fa7a1ab6ca0fb1b77b573980ca2f9dc72e3ac63232ca6978
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:8-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:c03b4386434dd75e35dd380fe391769b026b5b399caa8190ef3d09b148708503
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.1 MB (204131029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc0efa429ba929a9da90dfc50159ca888332207f63ff684e140524eeb8f736d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 05:18:44 GMT
SHELL [cmd /s /c]
# Sat, 18 Dec 2021 07:41:13 GMT
ENV JAVA_HOME=C:\openjdk-8
# Sat, 18 Dec 2021 07:41:13 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 07:41:22 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH% 	&& echo Complete.
# Sat, 18 Dec 2021 07:41:23 GMT
USER ContainerUser
# Sat, 18 Dec 2021 07:41:23 GMT
ENV JAVA_VERSION=8u312
# Sat, 18 Dec 2021 07:41:39 GMT
COPY dir:3a5581b2700e30ac96b7aaa667bdc25cdca1d6451f9f3d58913682ddf8d74e71 in C:\openjdk-8 
# Sat, 18 Dec 2021 07:41:53 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version 	&& echo Complete.
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4c557aac927613dd487d7c04b01a8eeb8ad174693f61b14c8f4285f1db6afdd2`  
		Last Modified: Sat, 18 Dec 2021 06:13:05 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9733ab20bd15f34d4ed6703746f020c819175941cb72305497495c8abaf2c0`  
		Last Modified: Sat, 18 Dec 2021 11:33:16 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6acc1717bc815d08bf7eaa5026823af817e8e0a50e64813a904715789c06d61`  
		Last Modified: Sat, 18 Dec 2021 11:33:15 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebf8621d074aabd74eec1769f2e45a0b21fac6ad6e21d33eb4719aaa117ac69`  
		Last Modified: Sat, 18 Dec 2021 11:33:13 GMT  
		Size: 67.2 KB (67188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811446d2e675afc4c0ec04fb2d6b7fe07ad0b1c99379b83355ceac9da741e6df`  
		Last Modified: Sat, 18 Dec 2021 11:33:13 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2cf16bb062589a2fb856b68fa8901b6b705bacd360b7425f79655100f9a00e`  
		Last Modified: Sat, 18 Dec 2021 11:33:13 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c2c43f52813bcc6454e4310e6949dd1fc29c0df03404a3b533bb168bf279f92`  
		Last Modified: Sat, 18 Dec 2021 11:33:26 GMT  
		Size: 101.1 MB (101073590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9283c63abc043b74e59d22f54f1996f7e5020fd7996a18b6e1f684f9772003c5`  
		Last Modified: Sat, 18 Dec 2021 11:33:13 GMT  
		Size: 80.4 KB (80440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
