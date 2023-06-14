## `eclipse-temurin:20-jdk-nanoserver-1809`

```console
$ docker pull eclipse-temurin@sha256:f511fd7db37200398c830a96d364cd4cef1335a9ffb07dd2d3a6a3c6f98641e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `eclipse-temurin:20-jdk-nanoserver-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull eclipse-temurin@sha256:44978b97d1588338bd5742e88b19077a2827462b0302ce187f461f0d0e2b5364
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.5 MB (303485754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c218db59dd0fbc7b07e4684dc6ca32b5c81bcaefd33b4896fbe6130a410c1d2e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Thu, 08 Jun 2023 12:28:32 GMT
RUN Apply image 10.0.17763.4499
# Wed, 14 Jun 2023 17:41:42 GMT
SHELL [cmd /s /c]
# Wed, 14 Jun 2023 18:06:12 GMT
ENV JAVA_VERSION=jdk-20.0.1+9
# Wed, 14 Jun 2023 18:06:13 GMT
ENV JAVA_HOME=C:\openjdk-20
# Wed, 14 Jun 2023 18:06:14 GMT
USER ContainerAdministrator
# Wed, 14 Jun 2023 18:06:25 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Wed, 14 Jun 2023 18:06:26 GMT
USER ContainerUser
# Wed, 14 Jun 2023 18:06:42 GMT
COPY dir:f42e28541c92f419d16f8f9260ba58e12cc63ca253028a61fc42e8a28f91cd69 in C:\openjdk-20 
# Wed, 14 Jun 2023 18:06:57 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Wed, 14 Jun 2023 18:06:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:234d39d9b188e7f36d5a77b0d54990ea826551314b6703c83aef3ef20b1a7050`  
		Last Modified: Tue, 13 Jun 2023 19:06:23 GMT  
		Size: 104.4 MB (104397895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2364e413270ecc5b57d2596b092fb57b828229b59e810d9f345fc0d31ca535d`  
		Last Modified: Wed, 14 Jun 2023 18:26:46 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5383d811aabbb2805907b3a15e1035fbe6d36d6ff2baced872afe06c93d85a57`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa085cac7c91c46669d4f8f81573dd462e288a713b4499ff83a1c7d1b46a58e`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21dfcac3d53075ad26971a6d98b48737f821c4cce49b09243478ccbb037692d4`  
		Last Modified: Wed, 14 Jun 2023 18:35:23 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9503cf15848877aadb5fee8ed3896908826a4b1623697603a6c1d925f565ad02`  
		Last Modified: Wed, 14 Jun 2023 18:35:21 GMT  
		Size: 71.0 KB (71018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286588e2ded622d2806a7ee81d5dbfcfdfadfd2cb85980d16c15ead49ee8b0d5`  
		Last Modified: Wed, 14 Jun 2023 18:35:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a675dc5c48821676f620cc1cfff1932e2cddf9e60929acf9b992d41a27d18bf3`  
		Last Modified: Wed, 14 Jun 2023 18:35:41 GMT  
		Size: 195.3 MB (195274575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904d0ab1a83b019130b638e39242d09ad39ef902db6733ba5a7b696dcf856675`  
		Last Modified: Wed, 14 Jun 2023 18:35:22 GMT  
		Size: 3.7 MB (3735337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5e60cea872425db11f171c381bf3ec66867522901409c475263753f6dd3057`  
		Last Modified: Wed, 14 Jun 2023 18:35:21 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
