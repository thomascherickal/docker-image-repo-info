## `eclipse-temurin:18-jdk-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:1d3ba463296a8083b0349bd2ba4378bff92d324b925dfd9d5d6525330b0e647d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.707; amd64

### `eclipse-temurin:18-jdk-nanoserver-ltsc2022` - windows version 10.0.20348.707; amd64

```console
$ docker pull eclipse-temurin@sha256:2abdf41a11909109792587d0bba16ef0c837336e5ebd5f745fd9703cad88acfd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304251551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9346c77527420682f23848ef45fe641e8228e8f179a8677863770fad99131c87`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 05 May 2022 02:37:33 GMT
RUN Apply image 10.0.20348.707
# Wed, 11 May 2022 15:21:54 GMT
SHELL [cmd /s /c]
# Wed, 11 May 2022 15:26:29 GMT
ENV JAVA_VERSION=jdk-18.0.1+10
# Wed, 11 May 2022 15:26:30 GMT
ENV JAVA_HOME=C:\openjdk-18
# Wed, 11 May 2022 15:26:30 GMT
USER ContainerAdministrator
# Wed, 11 May 2022 15:26:41 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 11 May 2022 15:26:42 GMT
USER ContainerUser
# Wed, 11 May 2022 15:26:57 GMT
COPY dir:dd9b13d03f0f59427148f5f854823680c639cd938d50ff4813e6410f92c7aca7 in C:\openjdk-18 
# Wed, 11 May 2022 15:27:15 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 11 May 2022 15:27:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2c74f0842c5a8e9b80b9e2cf64e1ab10a6fa67951f28cff5fee060b88128564c`  
		Size: 117.7 MB (117687017 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c783ef8875d74b7e18cf09914325e131a525d4678bc9b243734768fdbcde89a2`  
		Last Modified: Wed, 18 May 2022 13:44:02 GMT  
		Size: 1.1 KB (1103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d136dfaf5ae7a851d8ea1efa3640d91012139c0f92483b78c3a9be76f27d6fdd`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0470945a9c0833003c1fc65d3ad2497db1049955e680861d181d817082c8491f`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237cc5aee4d5732a84f29974bd6a67d4505998acf73f70352dd540353981926d`  
		Last Modified: Wed, 18 May 2022 13:54:05 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb2b36d85adcba260435f5c6f962c7ccdbba274a95df2318ef4a7bc6dbf4dcd`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 76.1 KB (76145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46ca06f941a094e65b95e7e8c2bd2d3775c06217ef567cec0555dcdb1096740`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f88152ae950e2276bcd2938e5dd0d85aac8fbc98af9ec4c535669f492d19aa`  
		Last Modified: Wed, 18 May 2022 13:54:22 GMT  
		Size: 186.4 MB (186421865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f8fbe7e05f74577662cae5999a188c69fca0a21d95c15b2cb04d3f7576eeb7`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 59.6 KB (59617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f731c9be4e7db076cec50ee25ff0412eb347dae9834032060b07259f65347e18`  
		Last Modified: Wed, 18 May 2022 13:54:03 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
