## `eclipse-temurin:11-nanoserver-ltsc2022`

```console
$ docker pull eclipse-temurin@sha256:101fad87707a6ab878478e41a68de3b66e71e1b93d895e03f245f0437a2ad0c2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `eclipse-temurin:11-nanoserver-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull eclipse-temurin@sha256:f8bdc3977199b1cd66b9e0790a0268234401bb998d03920ed97efdf8df5f9bb7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.2 MB (313157410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd3326a1bbd6c05a3615f362989b61337abbac2c484c774763fe86ef9506726`
-	Default Command: `["jshell"]`
-	`SHELL`: `["cmd","\/s","\/c"]`

```dockerfile
# Wed, 21 Jun 2023 07:39:21 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 01:08:07 GMT
SHELL [cmd /s /c]
# Sat, 24 Jun 2023 01:09:40 GMT
ENV JAVA_VERSION=jdk-11.0.19+7
# Sat, 24 Jun 2023 01:09:41 GMT
ENV JAVA_HOME=C:\openjdk-11
# Sat, 24 Jun 2023 01:09:42 GMT
USER ContainerAdministrator
# Sat, 24 Jun 2023 01:09:53 GMT
RUN echo Updating PATH: %JAVA_HOME%\bin;%PATH%     && setx /M PATH %JAVA_HOME%\bin;%PATH%     && echo Complete.
# Sat, 24 Jun 2023 01:09:53 GMT
USER ContainerUser
# Sat, 24 Jun 2023 01:10:10 GMT
COPY dir:aa85dc89894032bdcf98e5da06633e8de4813537c791ddbe3fc8bdfa8596f8de in C:\openjdk-11 
# Sat, 24 Jun 2023 01:10:26 GMT
RUN echo Verifying install ...     && echo javac --version && javac --version     && echo java --version && java --version     && echo Complete.
# Sat, 24 Jun 2023 01:10:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d6e77b89ecdadfdd3ef274e9a235590c9cd4dc832939932eff32f93250571005`  
		Last Modified: Fri, 23 Jun 2023 07:43:32 GMT  
		Size: 120.0 MB (120028254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e4670fd4887a293528c25b0a38905146f1a4f5dedcb3fc1c433715f01faf42`  
		Last Modified: Sat, 24 Jun 2023 01:34:23 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71328532fe3e7c9a5b123f73fd88dd66aed81951658212fa82c3f81ad09e1fa5`  
		Last Modified: Sat, 24 Jun 2023 01:35:13 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf7254d80ed10cf22be8ca4b228566a08f2f74518f7e577779370cd662465b5`  
		Last Modified: Sat, 24 Jun 2023 01:35:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613dec9326bb21840e70e24320ff7edfa56e82381e34835a27c01969e463be7`  
		Last Modified: Sat, 24 Jun 2023 01:35:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02161c0d2c1a9ef9543954f1fb02a00b48ee2878872ed645cfc6b62e70ce70e`  
		Last Modified: Sat, 24 Jun 2023 01:35:11 GMT  
		Size: 75.9 KB (75945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7368a12cc6a47c7ca5060834684282b674bf3c5ffb1cdb6f3f4a1a06d13db9`  
		Last Modified: Sat, 24 Jun 2023 01:35:10 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c32b0570823c87de3ba6e83a9efdf9b4ba08095ef688fdebb7e7ff3eaac1a3`  
		Last Modified: Sat, 24 Jun 2023 01:35:29 GMT  
		Size: 193.0 MB (192983740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d228457f52f2dd38ffc474dd3bee3e5f5ad5051aba5071c0a6895721793031`  
		Last Modified: Sat, 24 Jun 2023 01:35:10 GMT  
		Size: 62.5 KB (62538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29f178b86372c0507503ce053c5e06f323011e497a09deedd9ba88fa2ef54ed`  
		Last Modified: Sat, 24 Jun 2023 01:35:10 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
