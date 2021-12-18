## `openjdk:8u312-jre-nanoserver`

```console
$ docker pull openjdk@sha256:33661c805008eace341eec3a3e9dd688cde756bd0a4bd20ec1574fffea33b9b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2366; amd64

### `openjdk:8u312-jre-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull openjdk@sha256:2ccf49aa31cf89140cd610bb34ab7f62bdce199d8c2761e2daed391883c6c4e1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141287168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:728a474016d9b6642ecbb8dcce7ba2c700dee5eabd22c5c0001d4911219c6422`
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
# Sat, 18 Dec 2021 07:47:09 GMT
COPY dir:d01eca1f47b40119ea7401e87f8309ebbb3c59555f496ebfb4562b12d58cd948 in C:\openjdk-8 
# Sat, 18 Dec 2021 07:47:21 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version 	&& echo Complete.
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
	-	`sha256:d4c1bdfebbad493ae9c76fd3dd2091dab18ffdb0c4ab283fdc987b49b74cc792`  
		Last Modified: Sat, 18 Dec 2021 11:35:08 GMT  
		Size: 38.2 MB (38229629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b5b2a144914e42b1ff9d6c38c17837639e3acd29dcd2c96ce31249eefdadfb`  
		Last Modified: Sat, 18 Dec 2021 11:35:01 GMT  
		Size: 80.5 KB (80540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
