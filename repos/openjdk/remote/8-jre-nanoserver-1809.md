## `openjdk:8-jre-nanoserver-1809`

```console
$ docker pull openjdk@sha256:c9d4ac221125ea6f0da98db58031accc11ec43cfe9c23aac2fba2e6f2d884c8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:8-jre-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:0b4c683cd6663b666bd3b358d660cc62b3ede022502d23040db20d37041e0ad5
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138459958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f0f8a6ff4479b0333ed691dc03f06885515c2c935e660ae3f83710d163e12f4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Tue, 07 Jul 2020 13:50:07 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jul 2020 01:54:43 GMT
SHELL [cmd /s /c]
# Wed, 15 Jul 2020 02:34:08 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 15 Jul 2020 02:34:09 GMT
USER ContainerAdministrator
# Wed, 15 Jul 2020 02:34:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 15 Jul 2020 02:34:25 GMT
USER ContainerUser
# Wed, 15 Jul 2020 02:34:26 GMT
ENV JAVA_VERSION=8u252
# Wed, 15 Jul 2020 02:38:43 GMT
COPY dir:efe8678d9be4067f8f1280960ef457f634d7198257f7398711cb683e771f08bd in C:\openjdk-8 
# Wed, 15 Jul 2020 02:38:56 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:dc95608099543221ef539391bfece5c1ce37b97af9da457f5990349cab028a12`  
		Size: 100.9 MB (100895619 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9f6486e4debac36806ed3527d9b1baea75c1a807e26baccdd0a2f521c814273f`  
		Last Modified: Wed, 15 Jul 2020 02:43:55 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635f616413e2ffeb2b698529474f16b802473016d0380fd29b21f12527e7006d`  
		Last Modified: Wed, 15 Jul 2020 02:54:29 GMT  
		Size: 888.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a9bf2169040f2fa44109296c3dc79cd3e81ec224a0a19ae4d74f3866e4bac3`  
		Last Modified: Wed, 15 Jul 2020 02:54:29 GMT  
		Size: 887.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1401126acf0a8e1002c19605d846794b2a2e714f7bc1293cddc58869c1dc38c2`  
		Last Modified: Wed, 15 Jul 2020 02:54:27 GMT  
		Size: 63.8 KB (63805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f29752410c44cda8c2ee96c26c8abfed12f174fd499396fae2c94332705efa3`  
		Last Modified: Wed, 15 Jul 2020 02:54:27 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d08ebf9c6a0bc880336bca1404fd533d6cb933aca2c24314ce8d981834f7fb`  
		Last Modified: Wed, 15 Jul 2020 02:54:27 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08338a6a0125d2df7fb28ab2acf1b35e13adb408445d284e65cafdaa876e179c`  
		Last Modified: Wed, 15 Jul 2020 02:55:37 GMT  
		Size: 37.4 MB (37420979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b752ad2968f51eb79ad51c14c9a79fe6e6be9eb7c94a8c4ceac3e3a2f2798de2`  
		Last Modified: Wed, 15 Jul 2020 02:55:31 GMT  
		Size: 75.1 KB (75116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
