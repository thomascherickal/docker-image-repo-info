## `openjdk:8u272-nanoserver-1809`

```console
$ docker pull openjdk@sha256:bfb9dfccfadd893f6dc906f1cf3380367b712f2db2273829d37d46ed61e3fe4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:8u272-nanoserver-1809` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:3ff30e16aab8a250aff9a2bb552384789be42794d9740e3403d203d0703e24ad
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.4 MB (202384907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4818222d59236eaa0c8f908b14b13f10b00615bd6d27c3761ad11fb0f9d045d6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Sat, 31 Oct 2020 05:10:43 GMT
RUN Apply image 1809-amd64
# Wed, 11 Nov 2020 17:53:16 GMT
SHELL [cmd /s /c]
# Wed, 11 Nov 2020 18:19:07 GMT
ENV JAVA_HOME=C:\openjdk-8
# Wed, 11 Nov 2020 18:19:08 GMT
USER ContainerAdministrator
# Wed, 11 Nov 2020 18:19:19 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH% 	&& setx /M PATH %JAVA_HOME%\bin;%PATH%
# Wed, 11 Nov 2020 18:19:19 GMT
USER ContainerUser
# Wed, 11 Nov 2020 18:19:20 GMT
ENV JAVA_VERSION=8u272
# Wed, 11 Nov 2020 18:19:48 GMT
COPY dir:ba26a6340c532ef3b44bc920e785f61bc958fcf1ecefd576f1438bebffc3afee in C:\openjdk-8 
# Wed, 11 Nov 2020 18:20:06 GMT
RUN echo Verifying install ... 	&& echo   javac -version && javac -version 	&& echo   java -version && java -version
```

-	Layers:
	-	`sha256:f1b217fe8837d4d85cb8228a52344d3504d7aa51ba30167a20a6a4cb80cdcaa0`  
		Size: 101.3 MB (101279682 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:41b7be9dc08821cf81d29b16e0df54f7f3e3aeaa6407f43520c6259f2d84b10c`  
		Last Modified: Wed, 11 Nov 2020 18:27:27 GMT  
		Size: 864.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5293ca96aa254135b70635ee048740d1a51f05e657d122eecbe31de2f03f476f`  
		Last Modified: Wed, 11 Nov 2020 18:40:08 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de4cd2f1948cfa64e2c85180f38d5b346ab75f64984579c353871c117e54200`  
		Last Modified: Wed, 11 Nov 2020 18:40:07 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68eb57f2f9c7bbec6e6dab23eeb8c07223ac79ccfe78fffdfe5f3e28de0373ad`  
		Last Modified: Wed, 11 Nov 2020 18:40:04 GMT  
		Size: 67.6 KB (67580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6560cbbc5021992b82fe5be8aed78e5e07d433aab28cc63b880d521249767`  
		Last Modified: Wed, 11 Nov 2020 18:40:05 GMT  
		Size: 866.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4deb130ff340cdcf7faf49495f959576583e69e951e5cc835332ff8b4e8f2759`  
		Last Modified: Wed, 11 Nov 2020 18:40:05 GMT  
		Size: 860.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c97fdb1539f518ab502a36867904d40d98e975f751e658cc4fe09ea24b4d2d`  
		Last Modified: Wed, 11 Nov 2020 18:40:17 GMT  
		Size: 101.0 MB (100972754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67543a6dd12c9201d950b31b31b9ed632ee7686c2fe899d17cf638f6a83d381c`  
		Last Modified: Wed, 11 Nov 2020 18:40:05 GMT  
		Size: 60.5 KB (60548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
