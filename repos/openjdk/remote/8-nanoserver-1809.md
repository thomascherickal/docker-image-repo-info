## `openjdk:8-nanoserver-1809`

```console
$ docker pull openjdk@sha256:1d4dc5c80b7ccd29e5b49f9aae60c97d1ab6ffb439601d210d013b709d16d485
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1339; amd64

### `openjdk:8-nanoserver-1809` - windows version 10.0.17763.1339; amd64

```console
$ docker pull openjdk@sha256:8c41214bb62e9d06ee05d78978046d59e56f7f94958cb8483ab111d1b866a7eb
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.8 MB (200795847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71c0fa3c2c57933ef5ce3736e158a7e54f3c80aabf9750dee4494fa9427750e2`
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
# Wed, 15 Jul 2020 02:34:58 GMT
COPY dir:ab479e12b22d2d8e4d7a7f2a7c1ce2c9a985b2211941ab66c77b1be78e3ec440 in C:\openjdk-8 
# Wed, 15 Jul 2020 02:35:16 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
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
	-	`sha256:d13d5a390d5e4d9eaabb75203e8996f75878a7e67da45006e46bbefff87c7ea8`  
		Last Modified: Wed, 15 Jul 2020 02:54:38 GMT  
		Size: 99.7 MB (99746748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713a3877507a8e634e571a2a07f521f55a5d5d10bde9d55f4a8ff9f8485a5a3e`  
		Last Modified: Wed, 15 Jul 2020 02:54:27 GMT  
		Size: 85.2 KB (85236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
