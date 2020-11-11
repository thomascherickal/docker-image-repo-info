## `openjdk:8-jre-nanoserver`

```console
$ docker pull openjdk@sha256:b588ba5c8071b23ea869234f4f75165f448198e43c1dfe6c8eed1fe11cb3e4fc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1577; amd64

### `openjdk:8-jre-nanoserver` - windows version 10.0.17763.1577; amd64

```console
$ docker pull openjdk@sha256:bec633a8c974e6e9ee87fae823eaafe7188f07be692698950287540bfab3d932
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139595950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c4538a00b5385dc95ec1401e2e88fdc73241bf9c8e8e19e5da1a50955c9f6bd`
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
# Wed, 11 Nov 2020 18:23:12 GMT
COPY dir:cbcfc3652aed057bcd6387f24201b1963f79bbe4e98f6b8927ff7925a8b991a5 in C:\openjdk-8 
# Wed, 11 Nov 2020 18:23:27 GMT
RUN echo Verifying install ... 	&& echo   java -version && java -version
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
	-	`sha256:8a9340ab45cbd1803da53e11962f2826fb59cda7ce2611bfdb588826dda6680d`  
		Last Modified: Wed, 11 Nov 2020 18:41:24 GMT  
		Size: 38.2 MB (38191735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107f9c965e20c35278cec83d3fda0e03cea122f1c58de6f3ba4212db4d631ffe`  
		Last Modified: Wed, 11 Nov 2020 18:41:19 GMT  
		Size: 52.6 KB (52610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
